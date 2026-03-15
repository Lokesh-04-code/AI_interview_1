# 🤖 Hakkuna Mattata AI Interview

[![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://reactjs.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)](https://fastapi.tiangolo.com/)
[![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![Groq](https://img.shields.io/badge/Groq-f3f3f3?style=for-the-badge&logo=groq&logoColor=black)](https://groq.com/)

Hakkuna Mattata is a next-generation AI hiring platform that leverages Large Language Models and Voice AI to conduct adaptive technical interviews. It goes beyond static resumes by probing for depth, catching contradictions, and delivering evidence-based hiring signals in minutes.

---

## 🔥 Key Features

### 🧠 Intelligent Skill Analysis
- **Automatic Extraction**: Parses resumes using Groq LLM to build a comprehensive skill profile.
- **Confidence Scoring**: Assigns weights to candidate skills based on experience and projects.
- **Adaptive Probing**: Dynamically generates interview questions targeting low-confidence or critical skill areas.

### 🎙 AI Voice Interview
- **Natural Conversations**: Powered by **ElevenLabs** for human-like interviewer voice synthesis.
- **Real-Time Transcription**: Uses **Groq Whisper** for near-instant speech-to-text processing.
- **Live Interaction**: Provides a seamless voice call experience with real-time transcripts.

### 🔍 Deep Technical Probing
- **Adaptive Depth**: Transitions from basic to advanced questions based on candidate responses.
- **Edge Case Testing**: Challenges candidates with complex scenarios to verify true technical mastery.
- **Skill Confidence Graph**: Real-time visualization of evaluated candidate expertise.

### 📊 Comprehensive Reporting
- **AI-Powered Evaluation**: Scores participants on Technical Accuracy, Depth, and Consistency.
- **Decision Support**: Generates instant evaluation reports based on interview performance.

---

## 🛠 Tech Stack

- **Frontend**: React.js, Vite, Vanilla CSS, Recharts (Data Visualization).
- **Backend**: FastAPI (Python), Uvicorn.
- **Database**: MongoDB Atlas via Motor (asynchronous driver).
- **AI Engines**: 
  - **Groq**: Llama 3 70B (Text generation) & Whisper (Speech-to-Text).
  - **ElevenLabs**: Text-to-Speech synthesis for the interviewer voice.
- **Authentication**: JWT-based secure session management.

---

## 🚀 Getting Started

### Prerequisites

- Node.js (v18+)
- Python (v3.10+)
- MongoDB connection string
- Groq API Key
- ElevenLabs API Key

### 1. Backend Setup

```bash
cd Hakkuna_Mattata_AI_Interview
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

Create a `.env` file in the root backend folder:
```env
GROQ_API_KEY=your_groq_key
ELEVENLABS_API_KEY=your_elevenlabs_key
MONGODB_URI=your_mongodb_connection_string
```

Run the backend:
```bash
uvicorn main:app --reload
```

### 2. Frontend Setup

```bash
cd Frontend
npm install
```

Create a `.env` (or `.ENV`) file in the `Frontend` folder:
```env
VITE_API_URL=http://localhost:8000
```

Run the frontend:
```bash
npm run dev
```

---

## 📁 Project Structure

```text
├── Frontend/                 # React source code
│   ├── src/
│   │   ├── pages/            # Application views (SignIn, VoiceScreen, etc.)
│   │   ├── services/         # API integration layer
│   │   └── context/          # Auth and Global state
├── Hakkuna_Mattata_AI_Interview/ # Backend source code
│   ├── main.py               # FastAPI entry point
│   ├── resume_parser/        # Groq-powered parsing logic
│   └── Voice_Screening/      # Audio processing & AI interaction logic
└── README.md
```

---

## 🔐 Demo Credentials

Use the following credentials to explore the platform without creating an account:
- **Email**: `S@gmail.com`
- **Password**: `123456`

*(Check the "🔑 Try Demo" button on the Landing page for instant access!)*
