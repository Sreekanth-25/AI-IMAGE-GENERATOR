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


Run the script in Google Colab or your local GPU environment:

bash
Copy
Edit
python main.py
Or in Google Colab, the app will auto-launch:

Click Load Fast Model to initialize Stable Diffusion

Enter a prompt and adjust generation settings

Click Generate Images Fast!

View outputs in the interactive gallery

Click Show History to see previous prompts

📌 Example Prompts
A majestic dragon flying over snow-capped mountains, fantasy digital art

Cyberpunk city skyline at night, neon glow, highly detailed

A cute puppy sitting on grass, photorealistic, golden hour lighting

An astronaut walking on Mars with Earth in the sky, 8k render

🧪 Output & Validation
Prompt accuracy: Excellent alignment between text and image

Generation speed: ~5 seconds per image (on Colab GPU)

Visual quality: Highly detailed outputs at all resolutions

Error handling: Clear messages if invalid inputs or model not loaded

Responsive UI with gallery and logs

📤 Output Format
Generated Images displayed in gr.Gallery

Status Info includes: seed, steps, guidance, size, generation time

Logs stored in:

🔹 Generation History

🔹 Activity Log


