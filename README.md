# Ember - Emotional Support Chatbot

A clean, prototype-friendly Python project scaffold for an AI emotional-support chatbot built using LangGraph.

## Overview

Ember is designed to provide empathetic, context-aware emotional support through a multi-agent system. The architecture uses LangGraph to orchestrate four specialized agents that work together to understand, remember, and respond to users with care and empathy.

## Architecture

### Agents

1. **Mood Interpreter Agent** - Analyzes user input to determine emotional state and mood
2. **Contextual Recall Agent** - Retrieves relevant past conversations and memories
3. **Conversation Agent (Ember Core)** - Generates empathetic responses using mood and context
4. **Snapshot Extraction Agent** - Extracts key incidents and updates user summary

### Workflow

The LangGraph workflow connects all agents in sequence:
```
User Input → Mood Interpreter → Contextual Recall → Ember Core → Snapshot Extractor → Response
```

### Project Structure

```
ember/
├── app.py                 # Entry point
├── graph/                 # LangGraph workflow definitions
├── agents/                # Agent implementations (placeholders)
├── prompts/               # Prompt templates
├── memory/                # Database and memory management
├── models/                # LLM initialization
└── utils/                 # Helper functions
```

## Setup

1. Install dependencies:
```bash
pip install -r requirements.txt
```

2. Configure environment variables (create `.env` file):
```
LLM_API_KEY=your_api_key_here
DATABASE_URL=your_database_url_here
```

3. Run the application:
```bash
python -m ember.app
```

## Development Status

This is a scaffold project with placeholder implementations. All agent logic, database connections, and LLM integrations need to be implemented.

## Future Development

- Implement agent reasoning logic
- Set up database schema and connections
- Integrate LLM providers
- Build chat UI backend
- Add vector store for semantic memory retrieval
- Implement conversation persistence

## Notes

- Keep implementations minimal and prototype-friendly
- Focus on clean separation of concerns
- All business logic is intentionally left as TODOs for incremental development

