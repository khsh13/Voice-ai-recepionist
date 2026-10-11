# Voice-ai-recepionist

AI Voice Receptionist 🎙️

An AI-powered voice receptionist built with LiveKit Agents, Python, an LLM, and Docker. It handles real-time voice conversations, answers business queries, collects caller information, and assists with appointment requests.

🚀 Features
Real-time voice conversations using LiveKit Agents.
LLM-powered responses using Ollama or a free-tier API.
Speech-to-text (STT) and text-to-speech (TTS) integration.
Receptionist tools for FAQs, appointments, and caller messages.
FastAPI backend with PostgreSQL.
Docker-based containerization and deployment.
Error handling, logging, and automated testing.
🛠️ Tech Stack
Voice AI: LiveKit Agents
Language: Python
LLM: Ollama / free-tier LLM API
Backend: FastAPI
Database: PostgreSQL
Deployment: Docker & Docker Compose
Speech: Compatible STT and TTS providers
🏗️ Architecture
Caller
  ↓
LiveKit Voice Agent
  ↓
STT → LLM → TTS
  ↓
Agent Tools
  ↓
FastAPI Backend
  ↓
PostgreSQL Database

📁 Project Structure
ai-voice-receptionist/
├── app/
│   ├── agent/       # Voice agent and prompts
│   ├── api/         # FastAPI endpoints
│   ├── services/    # Receptionist business logic
│   └── db/          # Database models and sessions
├── tests/
├── Dockerfile
├── docker-compose.yml
├── pyproject.toml
├── .env.example
└── README.md

⚙️ Getting Started

1. Clone the repository

git clone <your-repository-url>
cd ai-voice-receptionist


2. Configure environment variables

Create a .env file using .env.example and configure your LiveKit credentials, LLM, and database.

3. Install dependencies

uv sync


4. Run the voice agent

uv run lk agent dev


5. Start the Docker services

After configuring Docker Compose:

docker compose up --build -d
docker compose logs -f

🗺️ Roadmap
Implement real-time voice conversations.
Integrate a free or locally hosted LLM.
Build receptionist tools and REST APIs.
Add PostgreSQL persistence.
Containerize services with Docker.
Deploy to a cloud server.
Add testing, monitoring, and human handoff.
📚 References
LiveKit Agents
Ollama
FastAPI
Docker Compose
🎯 Goal

Build and deploy a modular, low-latency AI receptionist that combines real-time voice interaction, LLM reasoning, backend integrations, and production-ready containerization.

Status: In development.