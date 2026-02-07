# LangGraph Agentic Chatbot

LangGraph + Gradio chatbot that can call Tavily web search as a tool during conversation.

## Quick Start

```bash
git clone https://github.com/akileshjayakumar/langgraph-agentic-chatbot.git
cd langgraph-agentic-chatbot
python -m venv .venv
source .venv/bin/activate
pip install -r infra/requirements.txt
```

Create `.env` in the repo root:

```env
OPENAI_API_KEY=your_openai_api_key
TAVILY_API_KEY=your_tavily_api_key
OPENAI_MODEL=gpt-4
OPENAI_TEMPERATURE=0
```

Run locally:

```bash
python app/app.py
```

Open `http://localhost:7860`.

## Core Capabilities

- Conversational interface built with Gradio `ChatInterface`
- LangGraph workflow with tool routing (`chatbot -> tools -> chatbot`)
- Tavily search integration for web-backed responses
- Configurable model and temperature through environment variables

## Configuration

Required:

- `OPENAI_API_KEY`
- `TAVILY_API_KEY`

Optional:

- `OPENAI_MODEL` (default: `gpt-4`)
- `OPENAI_TEMPERATURE` (default: `0`)

## Usage Example

Try prompts like:

- `What are the latest updates on NVIDIA's new GPU?`
- `Give me today's top AI headlines.`

## Contributing and Testing

- Open an issue or PR with a focused change.
- Basic local validation: start the app with `python app/app.py` and verify chat + tool calls work.
- Docker path: `docker build -f infra/Dockerfile .`

## License

MIT. See `LICENSE`.
