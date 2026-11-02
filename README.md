# AI Study Assistant

Upload lecture slides and notes → extract content → summarize → quiz → schedule revision.
A personal knowledge assistant (Notion + ChatGPT + Drive) built for students.

## Stack
- Backend: Python, FastAPI
- Database: PostgreSQL (+ pgvector for embeddings)
- Frontend: Next.js (React)
- Deploy: Docker

## Roadmap
- [x] Phase 0 — Foundations: repo, stack, skeleton
- [ ] Phase 1 — Store: notes CRUD, file uploads, login
- [ ] Phase 2 — Extract & search: PDF/PPTX text, full-text search
- [ ] Phase 3 — AI: embeddings, RAG "ask my notes", summaries
- [ ] Phase 4 — Study tools: flashcards, quizzes, spaced repetition, reminders
- [ ] Phase 5 — Polish: mind maps, deployment, demo

## Run the backend
```bash
docker compose up -d db
cd backend && pip install -r requirements.txt
uvicorn app.main:app --reload
```
Open http://localhost:8000/docs
