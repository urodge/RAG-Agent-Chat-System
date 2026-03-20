# Rag-Agent-Chat-System
Built a chat-style Retrieval-Augmented Generation (RAG) system that answers 
user queries by retrieving relevant context from a daily-updated MySQL database 
and passing it to a local LLM for grounded responses.

Key highlights:
- LLM tool-calling to fetch real-time data from structured database
- FAISS vector search for semantic document retrieval
- FastAPI backend serving the chat interface
- Fully local — no OpenAI API dependency

Stack: Python · FAISS · LLM · FastAPI · MySQL

A chat-based Retrieval-Augmented Generation (RAG) system using:
- Local LLM via Ollama
- FastAPI backend
- MySQL database
- Basic chat UI

## Features
- Asynchronous tool call agent
- Daily updating data via OpenFDA API
- Simple HTML UI or API interface

## How to Run

1. Set up MySQL and load data via `data_pipeline/fetch_api_data.py`
2. Start Ollama: `ollama run mistral`
3. Run FastAPI: `uvicorn api.main:app --reload`

