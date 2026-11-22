# Tigrinya Translation Agent

An AI agent that translates English to Tigrinya, built with LangChain and the Claude API.

## Features
- **Tool use:** counts the words in each translation
- **Memory:** remembers the conversation, so follow-ups like "now say it to a woman" work
- **Structured output:** returns `english`, `to_man`, and `to_woman` fields
- **Dynamic prompts:** switches between formal and casual tone
- **Human-in-the-loop:** pauses for approval before running tools

## What I found
As a native Tigrinya speaker, I checked each translation by hand. The model sometimes
mixed in Amharic, so I added strict rules to the system prompt to keep it in Tigrinya.

## Tech
Python · LangChain · Claude API · Jupyter

## Run it
1. Add `ANTHROPIC_API_KEY=your_key` to a `.env` file
2. Open `tigrinya_agent.ipynb` in Jupyter and run the cells
