# Production-Style RAG Chatbot with Evaluation

A production-oriented Retrieval-Augmented Generation (RAG) chatbot built with Python. It demonstrates document ingestion, chunking, embeddings, FAISS semantic retrieval, grounded generation, source inspection, and evaluation.

## Features
- Document ingestion and chunking
- Semantic retrieval with FAISS
- OpenAI embeddings and grounded generation
- Source-aware answers
- Evaluation dataset and metrics
- Streamlit interface
- Automated tests

## Architecture
Knowledge Base -> Chunk -> Embed -> FAISS -> Retrieve -> Grounded LLM Answer -> Evaluation

## Project Structure
- `app.py` — Streamlit interface
- `config.py` — configuration
- `evaluate.py` — evaluation runner
- `rag/` — chunking, embeddings, retrieval and generation
- `data/` — knowledge base
- `evaluation/` — evaluation dataset
- `tests/` — automated tests

## Quick Start
Requires Python 3.10+ and an OpenAI API key.

```bash
python -m venv .venv
# Windows
.venv\Scripts\activate
pip install -r requirements.txt
```

Create `.env` from `.env.example`, configure the API key, then run:

```bash
streamlit run app.py
python evaluate.py
pytest -q
```

## Portfolio Focus
**RAG • LLM Applications • Semantic Search • Evaluation • Python • FAISS • Streamlit**

> Never commit API keys or other secrets.