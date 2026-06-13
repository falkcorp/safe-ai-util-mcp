<!-- file: .github/copilot-instructions.md -->
<!-- version: 1.0.0 -->
<!-- guid: a3f7c2e1-8b4d-4f9a-b6e5-d2c1a0f3e8b7 -->
<!-- last-edited: 2026-06-13 -->

# safe-ai-util-mcp — Additional Context

Org-wide coding standards (file headers, language rules, commit format) are at
**https://github.com/falkcorp/.github** and apply automatically to this repo.

For full project context: **CLAUDE.md** at the repo root.

## Project overview

MCP server for safe-ai-util — exposes AI-safe command execution tools via Model Context Protocol. Language: Python.

## Key directories

| Path | Purpose |
|---|---|
| `src/safe_ai_util_mcp/` | MCP server implementation (server.py, tools.py) |
| `tests/` | Smoke and tool tests |

## Critical constraints

- Set `COPILOT_AGENT_UTIL_BIN` env var to the `safe-ai-util` binary path before running
- Uses stdio transport for MCP communication
- Python venv required: `python -m venv .venv && . .venv/bin/activate && pip install mcp`
