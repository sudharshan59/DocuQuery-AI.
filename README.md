🤖 DocuQuery AI — Ask Smarter Questions About Any File, Video, or URL!
One-click AI-powered Q&A for PDFs, CSVs, Images, Videos, Audio, Web Pages & YouTube — powered by TinyLlama, Whisper, SentenceTransformers, and Gradio. Deploy seamlessly to Hugging Face Spaces or run locally with ease!

🔗 Open in Colab | 🚀 Try on Hugging Face Spaces | 🧠 GitHub Repo

🚀 Key Features
Format	Capability
📄 PDF	Clean text extraction via pdfplumber
📊 CSV	Structured data parsing
🖼️ Image	OCR with pytesseract
🎥 Video	Audio extraction + transcription
🎧 Audio	Transcription via Whisper
🌐 Web URL	Scraping + cleaning
▶️ YouTube	Auto-download + transcribe
🧠 AI-Powered Q&A
TinyLlama-1.1B-Chat — lightweight, fast, and surprisingly smart

MiniLM-L6-v2 — semantic search for relevant chunks

FAISS — blazing-fast similarity retrieval

Smart Caching — skip reprocessing for repeated files

🌈 Beautiful UI
Built with Gradio — intuitive, shareable, and production-ready

One-click deploy to Hugging Face Spaces or Google Colab

⚙️ Installation & Setup
✅ Option 1: Run in Google Colab (Beginner-Friendly)
Just click the badge above — everything installs automatically!

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
💡 GPU acceleration recommended for Whisper + TinyLlama

🧠 How It Works
Ingest — Extracts text from any source (OCR, Whisper, scraping, etc.)

Chunk & Embed — Splits text and creates vector embeddings

Retrieve — Finds top-k relevant chunks using FAISS

Generate — TinyLlama answers using retrieved context (RAG pipeline)

Cache — Hashes files to avoid reprocessing — saves time & GPU!

🎯 Use Cases
“Summarize this PDF in 3 bullet points”

“What are the key findings from this CSV?”

“What did the speaker say in this YouTube video?”

“Extract and explain the data from this image”

🤝 Contribute & Collaborate
We welcome your ideas and improvements!

🐞 Report bugs

💡 Suggest features

📖 Improve documentation

🆕 Add support for new formats

📜 License
MIT License — Free to use, modify, and distribute!

🙌 Built With Love Using
🤗 Hugging Face — Models & Spaces

🧠 OpenAI Whisper — Audio transcription

📥 yt-dlp — YouTube downloading

📄 pdfplumber — Clean PDF extraction

🎨 Gradio — Stunning UI in minutes
✍️ Created with ❤️ by Sudharshanmonith
🔧 Systems Architect | 🧠 ML/NLP Engineer | 🔐 Privacy-First Builder Crafting secure, scalable AI tools for real-world impact.

📬 Connect on GitHub 📢 Contributions & feedback welcome!
