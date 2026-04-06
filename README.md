# Parasmani Interview VoiceBot

This is a small project I built to experiment with voice-based AI interaction.

Instead of just typing into a chatbot, I wanted something where I can speak, get a response, and even hear it back. It also tries to give better answers by using some custom data instead of replying generically.

---

## What this project does

- You can talk to the system using your voice  
- Or switch to normal chat mode and type  
- It converts speech to text, processes it, and gives a response  
- The response is also converted back into audio  
- It can use some predefined data (PDFs) to answer more accurately  
- For current topics, it can fetch results from the web  

---

## How it basically works

When you give input:

- If it's voice → converted to text  
- Then the system checks what the question is about  
- Based on that, it may use:
  - personal data
  - company-related data
  - or web search  
- Then it generates a short answer  
- Finally, it plays the response as audio  

I tried to keep responses short and more direct instead of long explanations.

---

## Project structure

Parasmani_Interview_VoiceBot/

- `frontend.py` → Streamlit UI (handles voice + chat)
- `ai_agent.py` → main logic (RAG, routing, tools)
- `data/`
  - `paras_profile.pdf`
  - `100x_profile.pdf`
- `.env` → API keys

---

## Setup steps

Clone the repo:

git clone https://github.com/your-username/Parasmani_Interview_VoiceBot.git  
cd Parasmani_Interview_VoiceBot  

Create virtual environment:

python -m venv venv  
venv\Scripts\activate  

Install requirements:

pip install -r requirements.txt  

---

## Add API keys

Create a `.env` file:

OPENAI_API_KEY=your_openai_api_key  
TAVILY_API_KEY=your_tavily_api_key  

---

## Run the app

streamlit run frontend.py  

---

## Tech used

- Streamlit  
- OpenAI APIs (GPT, Whisper, TTS)  
- LangChain  
- FAISS  
- Tavily  

---

## Why I made this

Mostly to understand how different components work together:
- speech input/output  
- LLM responses  
- retrieval-based answers  
- simple agent logic  

Also wanted something a bit more interactive than a normal chatbot.

---

## Things I might improve later

- cleaner UI (right now it's basic)
- storing chat history properly
- better response control
- maybe deploy it online

---

## Author

Parasmani Yogi
