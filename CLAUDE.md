# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

**Commit Note:** When making commits, always add the line:

Co-authored-by: claude[bot] <209825114+claude[bot]@users.noreply.github.com>

## Common Commands

- **Run the server:**  
  `uv run uvicorn server:app --host 0.0.0.0 --port 8082 --reload`

- **Start the proxy quickly:**  
  `uvx claude-code-proxy`

- **Set up environment variables:**  
  Copy example: `cp .env.example .env`  
  Edit `.env` for API keys and model config (see README for options).

- **Install Claude Code client:**  
  `npm install -g @anthropic-ai/claude-code`

- **Connect Claude Code client to proxy:**  
  `ANTHROPIC_BASE_URL=http://localhost:8082 claude`

## Architecture Overview

- The proxy server receives requests in Anthropic's API format, translates them to OpenAI format (using LiteLLM), and forwards to OpenAI or Gemini based on environment config.
- Model mapping is controlled with env vars (`PREFERRED_PROVIDER`, `BIG_MODEL`, `SMALL_MODEL`), supporting OpenAI and Gemini models.
- Handles both streaming and non-streaming API calls, maintaining compatibility with Claude tools and clients.
- See README.md for complete environment and customization instructions.
- The server code is in `server/`, structured for FastAPI (see `server/fastapi.py` and `server/main.py`).
- Proxy supports OpenAI and Gemini models, mapping Claude's `haiku`/`sonnet` to chosen backends.
- Customization and troubleshooting are primarily via environment variables and server command-line usage.
- No `.cursor` or Copilot rules are present.
- Review and follow best practices outlined in the README.md for any special setup or integration notes.
