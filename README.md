# 🖼️ LocalDiffusion  
A local, high-quality Stable Diffusion image generator optimized for performance and realism.

## 📌 Overview
LocalDiffusion is a Python-based image generation project that runs **Stable Diffusion v1.5** locally with memory and performance optimizations.  
It supports CUDA acceleration, xFormers attention optimization, and advanced prompt customization for generating **ultra-realistic, cinematic images**.

---

## ✨ Features
- 🎨 **High-quality image generation** with detailed prompts.
- ⚡ **CUDA GPU acceleration** for faster rendering.
- 🧠 **Memory optimization** via CPU offload, attention slicing, and xFormers.
- 🛠 **Customizable prompts** with negative prompt filtering.
- 🎯 **Reproducibility** with manual seed setting.
- 🏗 **Kitbash-style, photorealistic renders** ideal for sci-fi and cyberpunk themes.

---

## 🖥️ Installation

### 1️⃣ Clone the repository
```bash
git clone https://github.com/atharvataras/LocalDiffusion.git
cd LocalDiffusion
```


### 2️⃣ Create a virtual environment using uv
```bash
uv sync
```
(Alternatively, you can use pip install if not using uv.)

### 🚀 Usage
```bash
jupyter notebook main.ipynb
```

### 🔧 Troubleshooting
**ImportError: cannot import name 'cached_download' → Update huggingface_hub:**

```bash
uv add huggingface_hub==0.19.4
```
- CUDA out of memory → Lower resolution or steps, or enable attention slicing.
- Slow performance → Ensure xFormers is installed and CUDA is being used.