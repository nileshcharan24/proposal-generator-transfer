# FMR Proposal Generator (baseline)

Web app that auto-generates sponsorship proposal PPTs and cover letters using Gemini.
This is a sanitised baseline/reference: see `FMR_PROJECT_PLAN.md` for the plan and
`FMR_TECH_SPEC.md` for the technical spec.

- `backend/`  FastAPI app (auth, proposals, admin, PPTX editing, LLM calls)
- `frontend/` React + Vite UI
- `resources/` templates, guideline docs, cluster descriptions (add your own logos under `resources/logos/`)

## Setup
1. Copy `.env.example` to `.env` and fill in your own values (never commit `.env`).
2. Backend: `pip install -r requirements.txt` then `uvicorn backend.main:app --reload`
3. Frontend: `cd frontend && npm install && npm run dev`

Change the default admin password and `JWT_SECRET` before deploying anywhere.
