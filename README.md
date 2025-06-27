#### 🧠 Zero-Shot AI Debate Bot
A fully functional web application that simulates AI-powered debates on any topic using Large Language Models (LLMs) and Retrieval-Augmented Generation (RAG). The platform generates structured, multi-perspective arguments (Pro and Con) with user interaction features like counterpoints, feedback, and scoring.

###🌐 Demo
Enter a debate topic and watch AI generate compelling opening statements, rebuttals, and conclusions from both sides — with like/dislike feedback and vote counts.

![one](https://github.com/user-attachments/assets/b732b6be-6b33-4021-9c67-fb235e45470a)
![two](https://github.com/user-attachments/assets/b2488205-deec-4b28-9bd2-c2ce7baaab1e)
![three](https://github.com/user-attachments/assets/798c194a-d4b0-4a33-bde6-c98eadc9f74c)
![four](https://github.com/user-attachments/assets/fdbb9f24-aabb-44a0-97ec-296f80d8ac75)

###🏗️ Project Structure
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
