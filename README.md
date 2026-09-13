# OpenStudy AI

A non-commercial educational/research prototype for analyzing academic and educational documents.

## Features
- PDF/TXT upload and text extraction
- Document chunking
- TF-IDF information retrieval
- Extractive document summaries
- FastAPI REST API
- SQLite metadata store
- Docker deployment
- Automated tests and GitHub Actions CI

## Quick start

```bash
python -m venv .venv
# Windows: .venv\Scripts\activate
# Linux/macOS: source .venv/bin/activate
pip install -r requirements.txt
uvicorn app.main:app --reload
```

Open http://127.0.0.1:8000/docs

### Docker

```bash
docker compose up --build
```

## API
- `GET /health`
- `GET /stats`
- `POST /documents/upload`
- `GET /documents`
- `GET /documents/{id}`
- `GET /documents/{id}/summary`
- `POST /search`

## Roadmap
- PostgreSQL
- Redis + background worker queue
- Sentence-transformer embeddings
- FAISS/vector database
- OCR for scanned PDFs
- Authentication
- Larger research datasets
- GPU-enabled NLP experiments
- Retrieval-quality evaluation

## Educational scope
This project is intended for student/research experimentation with document processing, NLP, information retrieval and scalable service architecture.

## License
MIT
