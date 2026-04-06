# 🎤 Parasmani Interview VoiceBot

An AI-powered **Voice + Chat Assistant** built using **Streamlit, OpenAI, and LangChain**, designed to simulate a smart, human-like conversational agent.

This project allows users to:
- 🎙️ Speak directly to the AI (Voice Mode)
- 💬 Chat via text (Chat Mode)
- 🧠 Get intelligent, context-aware responses using RAG (Retrieval-Augmented Generation)
- 🔊 Hear responses in natural AI-generated voice

---

## 🚀 Features

### 🎤 Voice Mode
- Record voice input directly in the browser
- Speech-to-text using OpenAI Whisper
- AI response converted back to speech (Text-to-Speech)

### 💬 Chat Mode
- Simple text-based interaction
- Same intelligent backend processing

### 🧠 Smart AI Brain
- Uses **LangChain + OpenAI GPT**
- Retrieval from:
  - Personal profile (`paras_profile.pdf`)
  - Company profile (`100x_profile.pdf`)
- Context-aware responses using vector database (FAISS)

### 🌐 Web Search (Conditional)
- Uses Tavily Search API
- Triggered only for:
  - Latest trends
  - Market updates
  - Current events

### 🧾 Memory
- Maintains short conversation history
- Improves contextual continuity

---

## 🏗️ Project Structure

Parasmani_Interview_VoiceBot/
│
├── frontend.py          # Streamlit UI (Voice + Chat)
├── ai_agent.py          # Core AI logic (RAG + Agent)
├── data/
│   ├── paras_profile.pdf
│   └── 100x_profile.pdf
├── .env                 # API keys
└── README.md

---

## ⚙️ Installation

### 1️⃣ Clone Repository
git clone https://github.com/your-username/Parasmani_Interview_VoiceBot.git  
cd Parasmani_Interview_VoiceBot

### 2️⃣ Create Virtual Environment
python -m venv venv  
venv\Scripts\activate   (Windows)

### 3️⃣ Install Dependencies
pip install -r requirements.txt

---

## 🔑 Environment Variables

Create a `.env` file in root:

OPENAI_API_KEY=your_openai_api_key  
TAVILY_API_KEY=your_tavily_api_key  

---

## ▶️ Run the App

streamlit run frontend.py

---

## 🧠 How It Works

1. **User Input**
   - Voice → Whisper → Text
   - OR direct text input

2. **AI Processing**
   - Query routing:
     - About Paras → Personal PDF
     - About Company → Company PDF
     - Current topics → Web search
   - Context injected into LLM

3. **Response Generation**
   - GPT model generates short, human-like answers

4. **Output**
   - Display text
   - Convert to speech (TTS)

---

## 🎯 Key Technologies

- **Frontend:** Streamlit  
- **LLM:** OpenAI GPT (gpt-4o-mini)  
- **Speech-to-Text:** Whisper  
- **Text-to-Speech:** OpenAI TTS  
- **Framework:** LangChain + LangGraph  
- **Vector DB:** FAISS  
- **Search Tool:** Tavily API  

---

## 🧩 Core Logic (AI Agent)

- Conditional RAG (Retrieval-Augmented Generation)  
- Smart query routing  
- Minimal memory for efficiency  
- Tool-based reasoning (ReAct Agent)  

---

## 📌 Use Cases

- Interview preparation assistant  
- Personal AI portfolio bot  
- Voice-based AI demo project  
- Smart resume chatbot  
- AI product prototype  

---

## ⚡ Future Improvements

- Multi-language support  
- Persistent chat history (database)  
- UI enhancements (chat bubbles, animations)  
- Deployment (Streamlit Cloud / AWS)  
- Real-time streaming responses  

---

## 👤 Author

**Parasmani Yogi**  

- AI Engineer | Deep Learning | NLP | Computer Vision  
- Focused on building real-world AI systems  

---

## ⭐ If you like this project

Give it a ⭐ on GitHub and share!

---
