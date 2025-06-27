# 🧠 Zero-Shot AI Debate Bot
A fully functional web application that simulates AI-powered debates on any topic using Large Language Models (LLMs) and Retrieval-Augmented Generation (RAG). The platform generates structured, multi-perspective arguments (Pro and Con) with user interaction features like counterpoints, feedback, and scoring.

## 🌐 Demo
Enter a debate topic and watch AI generate compelling opening statements, rebuttals, and conclusions from both sides — with like/dislike feedback and vote counts.

![one](https://github.com/user-attachments/assets/b732b6be-6b33-4021-9c67-fb235e45470a)
![two](https://github.com/user-attachments/assets/b2488205-deec-4b28-9bd2-c2ce7baaab1e)
![three](https://github.com/user-attachments/assets/798c194a-d4b0-4a33-bde6-c98eadc9f74c)
![four](https://github.com/user-attachments/assets/fdbb9f24-aabb-44a0-97ec-296f80d8ac75)

## 🏗️ Project Structure
<pre><code> 
zero-shot-ai-debate-bot/
├── backend/                 # FastAPI Backend
│   ├── app/
│   │   ├── main.py
│   │   ├── routes/
│   │   │   └── debate.py
│   │   ├── schema/
│   │   │   └── debate.py
│   │   ├── services/
│   │   │   └── debate_engine.py
│   │   └── utils/
│   │       └── rag_wikipedia.py
│   └── requirements.txt
├── frontend/                # React + Vite + Tailwind Frontend
│   ├── src/
│   │   ├── components/
│   │   │   ├── Header.jsx
│   │   │   ├── TopicInput.jsx
│   │   │   ├── DebateDisplayArea.jsx
│   │   │   ├── ArgumentColumn.jsx
│   │   │   ├── ArgumentCard.jsx
│   │   │   ├── OverallVoteCounter.jsx
│   │   │   └── Footer.jsx
│   │   ├── App.jsx
│   │   └── main.jsx
│   └── vite.config.js
└── README.md
</code></pre>

## ⚙️ Features
✅ Zero-Shot Topic Understanding
✅ Structured Debate Format
✅ Dual AI Personas (Pro vs. Con)
✅ Like/Dislike Feedback System
✅ Vote Counter Display
✅ FastAPI Backend with OpenRouter API
✅ Wikipedia Retrieval (RAG)

## ▶️ Frontend Setup
<pre><code> 
cd frontend
npm install
npm run dev
</code></pre>

## 🧠 Backend Setup (FastAPI)
<pre><code> 
cd backend
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
pip install -r requirements.txt
uvicorn app.main:app --reload
</code></pre>

## 🔁 API Endpoints
### POST /debate/
Request: 
<pre><code>
  {
  "topic": "Is AI dangerous?"
  }
</code></pre>

Response: 
<pre><code>
  {
  "topic": "Is AI dangerous?",
  "pro": {
    "opening": "...",
    "rebuttal": "...",
    "closing": "..."
  },
  "con": {
    "opening": "...",
    "rebuttal": "...",
    "closing": "..."
  }
}
</code></pre>

## 📦 Technologies Used
### Frontend
- React  
- Vite  
- Tailwind CSS  
- Axios  
- Lucide Icons  

### Backend
- FastAPI  
- Pydantic  
- OpenRouter / OpenAI API  
- Wikipedia API (for RAG)  


## 🤖 Author

**Team BotMinds**  
- Ishatva Singh Panwar  
- Pratham Bajaj  
- Hritvik Mohan  
- Keith Kaur Malli  

_B.E., NITTE Meenakshi Institute of Technology_
