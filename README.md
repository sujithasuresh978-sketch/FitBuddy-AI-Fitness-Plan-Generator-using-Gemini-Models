# FitBuddy: AI Fitness Plan Generator

FastAPI + Gemini + SQLite + Jinja2.

## Run in VS Code
1. Open this folder in VS Code (File > Open Folder).
2. Open the terminal (Ctrl+`) and run:
   ```
   python -m venv venv
   venv\Scripts\activate          # macOS/Linux: source venv/bin/activate
   pip install -r requirements.txt
   ```
3. Copy `.env.example` to `.env` and paste your Gemini API key (https://aistudio.google.com/apikey).
4. Start the server (or press F5 and pick "FitBuddy (FastAPI)"):
   ```
   uvicorn app.main:app --reload
   ```
5. Open http://127.0.0.1:8000 (app) and http://127.0.0.1:8000/docs (API).

Pages: `/` plan builder, `/view-all-users` coach dashboard.
API: `POST /generate-plan`, `POST /update-plan/{user_id}`, `GET /nutrition-tip?goal=`.
