# AI Research Assistant

This project is an AI-powered research assistant that leverages advanced language models and real-time web tools to generate structured research outputs. The agent can answer queries, search the web, summarize information, and save research results to a file.

## Features

- **Conversational AI**: Uses Anthropic's Claude 3.5 Sonnet model for high-quality, context-aware responses.
- **Web Search Integration**: Retrieves up-to-date information using DuckDuckGo and Wikipedia.
- **Structured Output**: Returns research results in a structured format (title, summary, sources, tools used).
- **Persistence**: Can save research outputs to a timestamped text file for later reference.

## Installation

1. **Clone the repository** and navigate to the project directory.

2. **Create and activate a virtual environment**:
   ```sh
   python -m venv venv
   # On Windows (PowerShell):
   .\venv\Scripts\Activate
   ```

3. **Install dependencies**:
   ```sh
   pip install -r requirements.txt
   ```

4. **Set up your environment variables**:
   - Create a `.env` file in the project root with your API keys:
     ```
     ANTHROPIC_API_KEY=your_anthropic_api_key_here
     ```

## Usage

Run the main agent script:
```sh
python src/main.py
```
You will be prompted to enter your research query. The agent will use its tools to gather and summarize information, then print and (optionally) save the results.

## Project Structure

- `src/main.py` — Main entry point for the agent.
- `src/tools.py` — Custom tool definitions for web search, Wikipedia, and saving output.
- `requirements.txt` — List of required Python packages.
- `.gitignore` — Excludes the virtual environment from version control.

## Dependencies

- langchain
- langchain-community
- langchain-openai
- langchain-anthropic
- python-dotenv
- pydantic
- wikipedia
- duckduckgo-search

## Notes

- Ensure you have valid API keys for Anthropic in your `.env` file.
- All research outputs are saved to `research_output.txt` in the project root.

---

For more information, see the [GitHub repository](https://github.com/Elly-su/ai-research-assistant.git). 