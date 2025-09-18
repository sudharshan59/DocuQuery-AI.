# 🤖 DocuQuery AI — Ask Questions About Any Document, Video, or URL!

**DocuQuery AI** is a lightweight, privacy-first RAG-based assistant that lets you ask intelligent questions about PDFs, CSVs, images, videos, audio, web pages, and YouTube links.  
Powered by **TinyLlama**, **Whisper**, **SentenceTransformers**, and **FAISS**, with a beautiful **Gradio** interface.

🔗 [Open in Colab](https://colab.research.google.com/github/sudharshan59/DocuQuery-AI/blob/main/docuquery_ai.ipynb)  
🚀 [Try on Hugging Face Spaces](https://huggingface.co/spaces/sudharshanmonith/DocuQuery-AI)  
🧠 [GitHub Repo](https://github.com/sudharshan59/DocuQuery-AI)

---

## 🚀 Features

✅ **Multi-Format Support**  
Upload or paste links to:
- 📄 PDFs (via `pdfplumber`)
- 📊 CSVs
- 🖼️ Images (OCR with `pytesseract`)
- 🎥 Local Videos (audio extracted + transcribed)
- 🎧 Audio Files (transcribed with `Whisper`)
- 🌐 Web URLs (scraped & cleaned)
- ▶️ YouTube Videos (auto-download + transcribe)

✅ **AI-Powered Q&A**  
- 🔍 Semantic search with `all-MiniLM-L6-v2`
- ⚡ Fast retrieval using `FAISS`
- 🧠 Context-aware answers via `TinyLlama-1.1B-Chat`
- 🧊 Smart caching — no reprocessing for repeated files

✅ **Gradio UI**  
- Intuitive, shareable interface
- One-click deploy to Hugging Face Spaces or Colab

---

## 🧠 RAG Architecture Overview

```mermaid
graph TD
    A[Input File/URL] --> B[Text Extraction]
    B --> C[Chunking & Embedding]
    C --> D[FAISS Retrieval]
    D --> E[TinyLlama Generation]
    E --> F[Answer Display in Gradio]
Ingest: Extracts text using OCR, Whisper, scraping, etc.

Embed: Chunks and embeds using SentenceTransformers

Retrieve: Top-k relevant chunks via FAISS

Generate: TinyLlama answers using retrieved context

Cache: File hashes prevent redundant processing

📦 Installation
✅ Option 1: Run in Google Colab
Click the badge above — everything installs automatically!

🖥️ Option 2: Run Locally
bash
# Clone the repo
git clone https://github.com/sudharshan59/DocuQuery-AI.git
cd DocuQuery-AI

# Install dependencies (CUDA 11.8+ recommended)
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
pip install transformers sentence-transformers faiss-cpu gradio PyPDF2 beautifulsoup4 requests pillow pytesseract pandas opencv-python pdfplumber
pip install git+https://github.com/openai/whisper.git
pip install yt-dlp

# Install system packages (Linux/WSL)
sudo apt-get update && sudo apt-get install -y tesseract-ocr ffmpeg libgl1 libglib2.0-0

# Launch the app
python docuquery_ai.py
🖥️ Usage
After launching, you'll see a Gradio link like:

Code
Public URL:.[LIVE](https://huggingface.co/spaces/sudharshan001/DocuQuery-AI)
Then:

📂 Upload a file or paste a URL

❓ Ask any question — e.g., “Summarize this in 3 bullet points”

💡 Get instant answers powered by TinyLlama + retrieved context

🎯 Example Queries
“What are the key findings in this PDF?”

“Summarize this YouTube video”

“Extract and explain the data from this image”

“What does this CSV reveal about trends?”

🙌 Contributing
We welcome contributions!

🐞 Report bugs

💡 Suggest features

📖 Improve documentation

🆕 Add support for new formats

Fork the repo and submit a PR!

📜 License
MIT License — Free to use, modify, and distribute.

🙏 Acknowledgements
🤗 Hugging Face — Models & Spaces

🧠 OpenAI Whisper — Audio transcription

📥 yt-dlp — YouTube downloading

📄 pdfplumber — Clean PDF extraction

🎨 Gradio — Stunning UI in minutes

✍️ Created with ❤️ by Sudharshanmonith
🔧 Systems Architect | 🧠 ML/NLP Engineer | 🔐 Privacy-First Builder Crafting secure, scalable AI tools for real-world impact.
