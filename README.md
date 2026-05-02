# MedAuth Sentinel  
### Autonomous Prior Authorization & Appeals Agent

> Veersa Hackathon 2026 — ABES Batch of 2027  

---

## 🚀 Overview

Prior authorization delays cost billions and slow down patient care.  
**MedAuth Sentinel** automates this process using AI agents that review requests in seconds — with full reasoning transparency.

---

## 🤖 3-Agent Pipeline

- **IntakeAgent** → Validates request data  
- **DecisionAgent** → Applies medical + policy rules  
- **CriticAgent** → Reviews and corrects decisions  

---

## 🧠 Key Idea

The system uses a **self-correcting critic loop**, making it truly agentic — it detects and fixes its own mistakes without human intervention.

---

## 🏗️ Tech Stack

| Layer       | Technology                      |
|------------|--------------------------------|
| LLM        | Groq (llama-3.3-70b-versatile) |
| Backend    | FastAPI + Python               |
| Frontend   | React + Tailwind CSS           |
| Data       | JSON (no database required)    |
| Orchestration | Custom Python pipeline     |
| Testing    | Pytest + REST Client           |

---

## ⚡ Features

- End-to-end prior authorization automation  
- Step-by-step reasoning trace  
- Self-correcting AI decisions  
- Live prompt editing (Prompt Studio)  
- Pre-built demo scenarios  
- Fully testable architecture  

---

## ▶️ Quick Start

### Prerequisites
- Python 3.11+
- Node.js 18+
- Groq API Key

### Setup

```bash
# Clone repository
git clone https://github.com/your-team/medauth-sentinel.git
cd medauth-sentinel

# Setup environment
cp .env.example .env
# Add your GROQ_API_KEY

# Install backend dependencies
pip install -r requirements.txt

# Generate data
python backend/generate_data.py

# Run backend
uvicorn backend.main:app --reload

# Run frontend
cd frontend
npm install
npm start
