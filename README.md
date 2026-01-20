# 🤖 Zephyr-7B AI Assistant with Memory & Gradio UI

A professional-grade AI Chatbot built using the **Zephyr-7B-Beta** model. This project features a persistent memory system, 4-bit quantization for efficiency, and a modern, custom-styled Gradio interface.



## ✨ Key Features
- ** Local Memory System:** Automatically saves user info (like name) in a `chatbot_memory.json` file to remember context across sessions.
- ** Efficient Loading:** Uses `4-bit quantization` (bitsandbytes) to run a 7B parameter model smoothly on a T4 GPU.
- ** Permanent Caching:** Downloads the model once and saves it locally to avoid re-downloading on every run.
- ** Real-time Streaming:** Text scrolls in real-time as the AI generates it, providing a smooth user experience.
- ** Custom UI:** A polished, modern dark/light themed interface built with Gradio and custom CSS.

## 🛠️ Tech Stack
- **Model:** [HuggingFaceH4/zephyr-7b-beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)
- **Framework:** Transformers, Accelerate, Bitsandbytes
- **Interface:** Gradio (Blocks API)
- **Environment:** Python / Google Colab

## 🚀 How to Run in Google Colab
1. Open the `.ipynb` file in Google Colab.
2. Change the Runtime to **GPU (T4)**.
3. Install dependencies by running the first cell:
   ```bash
   pip install transformers accelerate gradio bitsandbytes
