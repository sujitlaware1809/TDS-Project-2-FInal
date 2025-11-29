# LLM Analysis Agent

An AI-powered agent that solves various tasks using LangGraph and Google's Gemini model.

## Features

- Automated task solving using LLM agents
- Web scraping with Playwright
- FastAPI backend for task submission
- Docker support for easy deployment

## Setup

1. Clone the repository:
```bash
git clone https://github.com/sujitlaware1809/tds-project-2.git
cd tds-project-2
```

2. Install dependencies:
```bash
uv sync
```

3. Create a `.env` file:
```
EMAIL=your_email@example.com
SECRET=your_secret
GOOGLE_API_KEY=your_google_api_key
```

4. Run the application:
```bash
uvicorn main:app --host 0.0.0.0 --port 7860
```

## Docker Deployment

```bash
docker build -t llm-analysis-agent .
docker run -p 7860:7860 --env-file .env llm-analysis-agent
```

## API Endpoints

- `GET /` - Welcome message
- `GET /healthz` - Health check
- `POST /solve` - Submit task for solving

## HuggingFace Spaces

## License

MIT
