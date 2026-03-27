# RAG LLM System (Python + FastAPI)

🚀 **project demonstrating:**
- RAG (Retrieval-Augmented Generation) pipeline
- Multi-LLM support (Ollama, OpenAI, Azure)
- FAISS / Pinecone vector store
- Async, retry, and circuit breaker for robust LLM calls
- Dockerized for production-ready deployment

---

## Features

1. **Multi-LLM Factory**:  
   Switch LLM via `.env` without changing code (`OLLAMA`, `OpenAI`, `Azure`)

2. **Vector Stores**:  
   - Local FAISS for free  
   - Optional Pinecone integration via env vars

3. **Resilient LLM calls**:  
   - Async execution  
   - Retry with timeout  
   - Circuit breaker for failures

4. **Dockerized**:  
   Run anywhere with `docker-compose up --build`

---

## Architecture Overview

User Query  
↓  
FastAPI API Layer  
↓  
Retriever (FAISS / Pinecone)  
↓  
Relevant Chunks  
↓  
LLM (Ollama / OpenAI / Azure)  
↓  
Final Answer (Grounded in retrieved context)

---

## Quick Start

1. Clone repo:

```bash
git clone https://github.com/BackdoorSentient/genai_rag_service.git
cd genai_rag_service

License
MIT License © 2026 Aniket Waichal
