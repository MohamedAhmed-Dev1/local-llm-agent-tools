# Local LLM Agent Tools

Two MCP tools that turn a local LLM into a fully private AI agent — no cloud, no subscriptions, no data leaving your PC.

Built and tested with [LM Studio](https://lmstudio.ai/) + Gemma 4.

---

## What This Does

Local LLMs are private but limited — no internet, no file access, no way to act on the world.

These two tools fix that by plugging into LM Studio's MCP config:

| Tool | What it adds |
|---|---|
| `exa` | Web search — live data via Exa API |
| `file-access` | Read, edit, and create files on your PC |

---

## Prerequisites

- [LM Studio](https://lmstudio.ai/) installed
- [Node.js](https://nodejs.org/) installed (for `npx`)
- A free [Exa API key](https://exa.ai/) (for the web search tool only)

---

## Setup

1. Open LM Studio and navigate to your `mcp.json` file
2. Choose which tools you want from the files in this repo
3. Copy the content into your `mcp.json` under `"mcpServers"`
4. Restart LM Studio

If you want both tools at once, use `full-mcp-config.json` as a reference.

---

## Files

| File | Description |
|---|---|
| `exa-web-search.json` | Web search tool config |
| `file-access.json` | File read/write/create tool config |
| `full-mcp-config.json` | Both tools combined in one file |

---

## Notes

- For `file-access`, replace the placeholder path with the folder you want the LLM to access
- For `exa`, replace the placeholder with your own Exa API key — never share your real key publicly

---

## Author

Mohamed Ahmed — First-year CS student at FCAI, Cairo University.

[LinkedIn](https://www.linkedin.com/in/mohamed-ahmed-031266221?utm_source=share_via&utm_content=profile&utm_medium=member_android)
