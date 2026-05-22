# Code Review Assistant

An AI-powered Python code review tool built with FastAPI and Claude API.
Paste any Python code and receive instant structured feedback across four categories.

## Live Features

- Bug detection — logical errors and runtime issues
- Security analysis — injection risks, hardcoded credentials, unsafe operations
- Code quality review — naming, error handling, documentation gaps
- Actionable suggestions — specific improvements with examples

## Tech Stack

- **Backend:** Python, FastAPI, Anthropic Claude API
- **Frontend:** HTML, CSS, Vanilla JavaScript
- **AI Model:** Claude Sonnet (claude-sonnet-4-20250514)
- **Deployment:** Render (backend), static HTML (frontend)

## Project Structure

code-review-assistant/
├── backend/
│   ├── main.py          # FastAPI server and routes
│   ├── reviewer.py      # Claude API integration and prompt engineering
│   ├── requirements.txt
│   └── .env             # API keys (never committed)
├── frontend/
│   ├── index.html       # Main UI
│   ├── style.css        # Styling
│   └── script.js        # API calls and DOM rendering
└── README.md

## How to Run Locally

**1. Clone the repository**
```bash
git clone https://github.com/yourusername/code-review-assistant.git
cd code-review-assistant
```

**2. Set up the backend**
```bash
cd backend
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```

**3. Add your API key**

Create a `.env` file inside the backend folder: 

ANTHROPIC_API_KEY=your_key_here

**4. Run the server**
```bash
uvicorn main:app --reload
```

**5. Open the frontend**

Open `frontend/index.html` directly in your browser.

## Usage

1. Paste any Python code into the editor
2. Click **Review My Code** or press **Ctrl + Enter**
3. Receive structured feedback across four categories instantly

## What I Learned

- Prompt engineering to force structured JSON output from LLMs
- Building REST APIs with FastAPI and Pydantic validation
- Connecting a vanilla JS frontend to a Python backend via fetch
- Handling LLM response parsing and error states gracefully
- CORS configuration for local development

## Author

**PVS Deepak** — B.E. Computer Science, CBIT Hyderabad  
[LinkedIn](https://www.linkedin.com/in/pvs-deepak-7b095a335?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app) | [Github](https://github.com/PVSDEEPAK)