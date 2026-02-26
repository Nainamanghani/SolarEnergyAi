---
title: Energy Agent
emoji: ⚡
colorFrom: blue
colorTo: indigo
sdk: docker
pinned: false
---

# ⚡ Energy Agent  
### Autonomous Energy Research & Analysis AI Agent

Energy Agent is an AI-powered autonomous agent designed to research, analyze, and generate insights on energy-related topics.  
It leverages modern AI tools and agent-based workflows to assist in smart energy decision-making.

---

Before running the project, ensure you have:

- Python **3.10+**
- API Keys:
  - LLM Provider (Groq / OpenAI / other)
  - Tavily API (for web search)

---

## ⚙️ Installation & Setup

1️⃣ Clone the Repository

git clone https://github.com/Nainamanghani/SolarEnergyAi
cd SolarEnergyAi

2️⃣ Create a Virtual Environment
Windows

python -m venv venv
.\venv\Scripts\activate


3️⃣ Install Dependencies

pip install -r requirements.txt
 Environment Variables

This project requires API keys for LLM and Search.

Create a .env file in the root directory:

GROQ_API_KEY=your_groq_api_key_here
TAVILY_API_KEY=your_tavily_api_key_here

▶️ Running the Application

Run the Agent
python main.py

(If backend/frontend are separated, update this section accordingly)

You need to run the **Backend** and **Frontend** in two separate terminals.

### 1. Start the Backend (FastAPI)
Open a new terminal, activate the venv, and run:
```bash
python -m uvicorn backend.main:app --reload
```
The API will start at `http://localhost:8000`.

### 2. Start the Frontend (Streamlit)
Open another terminal, activate the venv, and run:
```bash
python -m streamlit run frontend/app.py
```
The UI will automatically open in your browser at `http://localhost:8501`.

✨ Features

 Autonomous AI agents for energy research

 Web-based research using Tavily

 Structured analysis & report generation

 Multi-agent workflow (Researcher, Analyst, Writer)

 Persistent knowledge storage


 Project Structure
Energy_agent/
│
├── backend/
│   ├── main.py
│   ├── knowledge_base/
│
├── frontend/
│   ├── app.py
│
├── requirements.txt
├── .env.example
├── README.md


(Structure may vary depending on implementation)

🧰 Tech Stack
Backend

Python

FastAPI

LangChain

Pydantic

Frontend

Streamlit

Tools & AI

CrewAI

Tavily (Search)

LLM APIs (Groq / OpenAI)