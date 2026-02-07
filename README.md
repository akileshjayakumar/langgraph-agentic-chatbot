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

## Capabilities
- Conversational interface built with Gradio `ChatInterface`
- LangGraph workflow with tool routing (`chatbot -> tools -> chatbot`)
- Tavily search integration for web-backed responses
- Configurable model and temperature through environment variables

## Configuration
- `OPENAI_API_KEY`: Required for related integrations/features.
- `OPENAI_MODEL`: Required for related integrations/features.
- `OPENAI_TEMPERATURE`: Required for related integrations/features.
- `TAVILY_API_KEY`: Required for related integrations/features.

## Usage
```bash
ls -la
```

## Contributing and Testing
- Contributions are welcome through pull requests with clear, scoped changes.
- No automated test suite is currently documented for this repository.

## License
Licensed under the `MIT` license. See [LICENSE](./LICENSE) for full text.
