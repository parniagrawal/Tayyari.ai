# 🧠 Tayyari.ai — AI-Powered Learning & Assessment Assistant

Tayyari.ai is an intelligent, multimodal education assistant designed to enhance self-paced learning using cutting-edge AI technologies. It supports personalized content summarization, text-to-speech learning, speech-to-text transcription, and interactive Q&A — all powered by Gemini Pro, Whisper, and LangChain.

## 🚀 Features

- 📄 **Document & Note Ingestion**: Upload PDFs or enter custom notes to process and summarize.
- 🤖 **Gemini Pro Integration**: Uses Gemini's `generateContent` API to create interactive learning modules.
- 🔊 **Text-to-Speech (TTS)**: Converts content into spoken audio using Kokoro or GTTS.
- 🗣️ **Speech-to-Text**: Records user speech and transcribes using OpenAI's Whisper model.
- ❓ **Explain More**: Dive deeper into concepts with context-aware explanations.
- 🎯 **Interactive Questions**: Generate MCQs dynamically to test user understanding.
- 🧠 **FAISS-based RAG**: Uses LangChain with FAISS vector store for smart context retrieval.
- 🌐 **Frontend Integration**: Built to work seamlessly with a React/Next.js frontend (localhost:3000).

## 📦 Tech Stack

| Layer        | Tools Used                                     |
|--------------|------------------------------------------------|
| Backend      | Python, Flask, LangChain, FAISS                |
| AI Services  | Gemini Pro API (Google), OpenAI Whisper        |
| NLP & Audio  | pdfplumber, soundfile, gTTS, Kokoro            |
| Frontend     | React / Next.js (assumed), Axios               |
| Deployment   | Vercel (Frontend), Local Flask Server          |

## ⚙️ Setup Instructions

1. Clone the Repository
   ```bash
   git clone https://github.com/parniagrawal/Tayyari.ai.git
   cd Tayyari.ai/backend
2. Set up Virtual Environment
python -m venv venv
venv\Scripts\activate  # On Windows

4. Install Dependencies
pip install -r requirements.txt

5. Set Up Environment Variables
Create a .env file in the backend/ directory:
GEMINI_API_KEY=your_gemini_api_key_here

6. Run the Flask Server
python app.py

🛠 Troubleshooting
❌ ModuleNotFoundError: Ensure all dependencies are installed with pip install -r requirements.txt.
❌ CORS Error: Double-check that your frontend is running on http://localhost:3000.
❌ Whisper Error: Ensure ffmpeg is installed and added to your system path.

🧪 Future Enhancements
Add user authentication (OAuth or Firebase)
Deploy backend to Render / Railway
Use persistent database (e.g., PostgreSQL) for chat/session tracking
Add analytics dashboard to track user progress

🙌 Contributors
Parni Agrawal
Shrey Joshi
Kumaran Hariharan
Shatakshi Singh
And the amazing team contributing to this project ❤️

