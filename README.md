# 🖼️ ComfyUI + Gradio Image Editing Interface

This repository provides a **streamlined integration** between [ComfyUI](https://github.com/comfyanonymous/ComfyUI) and [Gradio](https://gradio.app/) to create an elegant **web-based interface** for image manipulation.

The included Python script wraps the ComfyUI pipeline in a modern, user‑friendly Gradio front‑end — enabling you to control prompt text, sampling steps, CFG scale, and image inputs directly from your browser.

---

## ✨ Features

- **ComfyUI Workflow Integration**:
  - Loads and configures the following:
    - **Model:** Qwen Image Edit Q8 GGUF
    - **CLIP Loader:** Qwen 2.5
    - **VAE:** QWE Image VAE
    - **LoRA:** Qwen Image Edit LoRA (Lighting enhancement, 8 steps)
- **Web UI Powered by Gradio**:
  - Black background **dark mode** for less eye strain.
  - Side‑by‑side controls and output preview.
  - Sliders for **steps** and **CFG scale**.
  - Image upload with automatic resizing to 512px minimum side.
- **Automatic Output Detection**: Returns the newest generated image after processing.

---

## 📂 Repository Structure
├── app.py # Main Gradio + ComfyUI integration code 


├── Image Editing Qwen (1).json # ComfyUI workflow JSON file 


├── input/ # Uploaded images (auto-created) 


├── output/ # Generated images from ComfyUI 

---

## 🚀 Getting Started

### 1️⃣ Prerequisites
- Python 3.9+
- [ComfyUI](https://github.com/comfyanonymous/ComfyUI) installed and configured
- `pip install gradio pillow numpy pandas` 
-  Ensure you have the following models in your ComfyUI models/ folder:
-  Qwen Image Edit Q8 GGUF
-  Qwen 2.5 CLIP
-  QWE Image VAE

Qwen Image Edit LoRA (8-step lighting version)
### 2️⃣ Clone This Repository
```bash
git clone https://github.com/YourUsername/comfyui-gradio-image-edit.git
cd comfyui-gradio-image-edit

