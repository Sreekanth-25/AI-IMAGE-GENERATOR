# 🎨 AI-Based Image Generator

🧠 **Text-to-Image Generator using Stable Diffusion**

This project is an AI-powered image generation app that uses **Hugging Face Diffusers**, **Gradio**, and **Stable Diffusion v1.5** to create high-quality images from user prompts. The interface allows users to adjust parameters like resolution, guidance scale, batch size, and more — with real-time generation and a rich visual gallery.

---

## 🚀 Features

- ✏️ **Enter your own image prompt**  
- 🖼️ **Resolution control**: 256 to 1024 pixels  
- 🔁 **Batch generation**: 1–4 images per prompt  
- 🎛️ **Adjust steps and guidance scale**  
- 🎲 **Seed control** for reproducibility or randomness  
- ⚙️ **Optimized GPU usage** using attention slicing and xformers (if available)  
- 📜 **Prompt history** and **activity log** tracking  
- 🖥️ **Gradio Blocks-based interface** with custom styling  
- 🌐 **Public URL** via Colab for easy sharing

---

## 🛠️ Tech Stack

| Tool / Library            | Purpose                              |
|---------------------------|--------------------------------------|
| 🧠 Hugging Face Diffusers | Stable Diffusion pipeline            |
| 🎨 Gradio (Blocks)        | Web UI and user interaction          |
| 🔄 DPMSolver Scheduler    | Faster inference with better results |
| 🖥️ Google Colab           | GPU execution and deployment         |
| 🐍 Python                 | Core application logic               |
| 📦 Torch / Xformers       | Model execution & memory efficiency  |

---

## 📦 Installation (Colab Setup)

### 🔧 Prerequisites

- Python 3.8+
- Google Colab with GPU enabled (Recommended: T4)
- Internet connection to fetch models

### 📥 Setup Instructions

```bash
!pip install --upgrade pip
!pip install gradio==3.50.2
!pip install diffusers transformers accelerate torch torchvision pillow xformers -q
!pip install --upgrade huggingface_hub
