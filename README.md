🤖 DocuQuery AI — Ask Questions About Any Document, Video, or URL!
One-click AI-powered Q&A for PDFs, CSVs, Images, Videos, Audio, Web Pages & YouTube!
Powered by TinyLlama, Whisper, SentenceTransformers, and Gradio — deployable to Hugging Face Spaces! 

Open In Colab

Hugging Face Spaces

Python 3.8+

License: MIT

🚀 Features
✅ Multi-Format Support — Upload or paste links to:

📄 PDFs (with pdfplumber for clean text)
📊 CSVs
🖼️ Images (OCR via pytesseract)
🎥 Local Videos (audio extracted + transcribed)
🎧 Audio Files (transcribed with Whisper)
🌐 Web URLs (scraped & cleaned)
▶️ YouTube Videos (auto-download + transcribe!)
🧠 AI-Powered Q&A using:

TinyLlama/TinyLlama-1.1B-Chat-v1.0 — fast, lightweight, surprisingly smart!
all-MiniLM-L6-v2 — for semantic retrieval
FAISS — for lightning-fast similarity search
⚡ Smart Caching — Same file? No reprocessing!
🌐 Gradio UI — Beautiful, intuitive, shareable interface
☁️ One-Click Deploy — Ready for Hugging Face Spaces or Colab!

📦 Installation & Setup
Option 1: Run in Google Colab (Recommended for Beginners)
👉Open In Colab

Just click the badge above — everything installs automatically!

Option 2: Run Locally

# Clone the repo
git clone https://github.com/yourusername/docuquery-ai.git
cd docuquery-ai

# Install dependencies (CUDA 11.8 recommended)
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
pip install transformers sentence-transformers faiss-cpu gradio PyPDF2 beautifulsoup4 requests pillow pytesseract pandas opencv-python pdfplumber
pip install git+https://github.com/openai/whisper.git
pip install yt-dlp

# Install system packages (Linux/WSL)
sudo apt-get update && sudo apt-get install -y tesseract-ocr ffmpeg libgl1 libglib2.0-0

# Run the app
python docuquery_ai.py

💡 Note: For GPU acceleration, ensure you have CUDA 11.8+ and compatible drivers. 

🖥️ Usage
Launch the App — After running, you’ll see a Gradio link like:


1
Public URL: https://xxx-xxx-xxx.gradio.live
Upload or Paste:
📂 Upload a file (PDF, CSV, image, video, audio)
🌐 Paste a URL (supports YouTube!)
❓ Ask Any Question — e.g., “Summarize this in 3 bullet points” or “What are the key findings?”
💡 Get Instant AI Answers — Powered by TinyLlama with retrieved context!
🎥 Demo Preview
DocuQuery AI Interface

(Replace with actual screenshot when available)

🧠 How It Works
Ingest → Extracts text from any source (OCR, Whisper, scraping, etc.)
Chunk & Embed → Splits text and creates vector embeddings
Retrieve → Finds top-k relevant chunks using FAISS
Generate → TinyLlama answers using retrieved context (RAG pipeline)
Cache → Hashes files to avoid reprocessing — saves time & GPU!
🤝 Contributing
Contributions are welcome! Please fork the repo and submit a PR.

Report bugs 🐞
Suggest features 💡
Improve documentation 📖
Add new file format support 🆕
📜 License
MIT License — Feel free to use, modify, and distribute!

🙌 Acknowledgements
Hugging Face 🤗 — Models & Spaces
OpenAI Whisper — Audio transcription
yt-dlp — YouTube downloading
pdfplumber — Superior PDF text extraction
Gradio — Beautiful UI in minutes
