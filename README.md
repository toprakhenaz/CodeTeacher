# CodeTeacher

## 🚀 Usage Guide

### 1. Installation & Setup

```bash
# Install required packages
pip install gradio transformers torch accelerate bitsandbytes

# Run the application
python KullaniciArayuzu.ipynb
```

Or use **Google Colab** for GPU access (recommended).

### 2. Getting Started

#### Step 1: Select a Model
Choose from 6 available models in the dropdown:

**Toprak Henaz Models:**
- DeepSeek Coder 6.7B (ToprakH) - Best for code generation
- CodeLlama Magicoder 7B (ToprakH) - Great for code completion
- Gemma 7B (ToprakH) - General purpose model
- Qwen2.5 Coder 7B (ToprakH) - Advanced code analysis

**ByGedik Models:**
- Llama 3.1 8B CodeAlpaca (ByGedik) - Excellent code explanations
- Mistral CodeAlpaca V3 (ByGedik) - Quality code examples

#### Step 2: Load the Model
1. Click **"📥 Model Yükle"** to load your selected model
2. Wait for confirmation message: "✅ Model başarıyla yüklendi!"
3. The model is now cached and ready to use

#### Step 3: Enter Your Prompt
Write your coding question or request in the prompt box. Examples:
```
Python'da bir fibonacci fonksiyonu yaz ve açıkla
JavaScript ile REST API çağrısı nasıl yapılır?
SQL ile JOIN işlemleri örneği
React functional component ile state management
```

#### Step 4: Adjust Parameters (Optional)
- **📏 Maksimum Uzunluk**: 50-1024 tokens (default: 512)
- **🌡️ Temperature**: 0.1-2.0 (default: 0.7)
  - Lower = more consistent, Higher = more creative
- **🎯 Top-p**: 0.1-1.0 (default: 0.9)
  - Controls word choice diversity

#### Step 5: Generate Response
Click **"🚀 Üret"** and get your AI-generated response!

### 3. Advanced Features

#### 🔄 Model Switching
- **Smart Cache**: Up to 3 models cached simultaneously
- **Instant Switch**: Change between cached models in <1 second
- **Memory Management**: Automatic cleanup of oldest models

#### 📦 Cache Management
- **"📦 Cache Durumu"**: Check current cached models
- **"🗑️ Bu Modeli Sil"**: Remove specific model from cache
- **"🧹 Tümünü Temizle"**: Clear all cached models

#### 🎯 Model Comparison
Test the same prompt across different models to compare:
1. Load Model A, enter prompt, generate
2. Switch to Model B (cached), same prompt, generate
3. Compare results instantly!

### 4. Usage Tips

#### 💡 Best Practices
- **Start with DeepSeek-Coder** for general code generation
- **Use CodeLlama** when you need creative/diverse solutions
- **Try Qwen2.5-Coder** for complex code analysis
- **Cache 2-3 models** you use frequently
- **Adjust temperature** based on task:
  - Code generation: 0.3-0.7
  - Creative writing: 0.7-1.2
  - Problem solving: 0.5-0.9

#### 🚀 Performance Optimization
- **GPU Recommended**: Much faster generation
- **4-bit Quantization**: Automatically applied for memory efficiency
- **Batch Processing**: Load multiple models for comparison
- **Memory Monitoring**: Use cache status to manage resources

#### 🎯 Prompt Engineering
**Good Prompts:**
```
✅ "Python'da binary search algoritması yaz ve her adımı açıkla"
✅ "React'te useState hook'u nasıl kullanılır? Örnek ver"
✅ "SQL'de INNER JOIN ve LEFT JOIN arasındaki fark nedir?"
```

**Avoid:**
```
❌ "Kod yaz" (too vague)
❌ "Program yap" (unclear requirements)
❌ "Help me" (no specific context)
```

### 5. Example Workflow

```python
# 1. Select Model
Model: "DeepSeek Coder 6.7B (ToprakH)"

# 2. Load Model
Click "📥 Model Yükle"
Status: "✅ DeepSeek Coder 6.7B başarıyla yüklendi!"

# 3. Enter Prompt
"Python'da quicksort algoritması yaz ve time complexity'sini açıkla"

# 4. Set Parameters
Max Length: 512
Temperature: 0.7
Top-p: 0.9

# 5. Generate
Click "🚀 Üret"

# 6. Get Result
def quicksort(arr):
    if len(arr) <= 1:
        return arr
    
    pivot = arr[len(arr) // 2]
    left = [x for x in arr if x < pivot]
    middle = [x for x in arr if x == pivot]
    right = [x for x in arr if x > pivot]
    
    return quicksort(left) + middle + quicksort(right)

# Time Complexity: O(n log n) average case, O(n²) worst case...
```

### 6. Troubleshooting

#### Common Issues & Solutions

**"❌ Model yüklenirken hata"**
- Check internet connection
- Ensure sufficient disk space (50GB+)
- Try different model

**"❌ Lütfen önce bir model seçin"**
- Load a model first using "📥 Model Yükle"
- Wait for confirmation message

**Slow Generation**
- Use GPU-enabled environment (Colab)
- Reduce max_length parameter
- Clear cache if memory full

**Poor Quality Output**
- Try different temperature values
- Improve prompt specificity
- Test with different models

### 7. System Requirements

**Minimum:**
- Python 3.8+
- 8GB RAM
- 50GB storage

**Recommended:**
- CUDA GPU (RTX 3060+)
- 16GB+ RAM
- 100GB+ SSD storage
- Stable internet connection

### 8. Support

**Quick Help:**
- Click examples below the prompt box
- Use "📦 Cache Durumu" to monitor system
- Try "🧹 Tümünü Temizle" if issues persist

**Performance Tips:**
- Keep max 3 models cached
- Use appropriate parameters for your task
- Monitor GPU memory usage
- Restart if experiencing memory issues

---

**🎯 Ready to start? Select a model, enter your prompt, and experience AI-powered code generation!**
