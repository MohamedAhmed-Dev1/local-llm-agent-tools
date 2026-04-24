# Local LLM Agent Tools

Three MCP tools that turn a local LLM into a fully private AI agent — no cloud, no subscriptions, no data leaving your PC.

Built and tested with [LM Studio](https://lmstudio.ai/) + Qwen3.5 4B.

---

## What This Does

Local LLMs are private but limited — no internet, no file access, no way to act on the world.

These three tools fix that by plugging into LM Studio's MCP config:

| Tool | What it adds |
|---|---|
| `exa` | Web search — live data via Exa API |
| `file-access` | Read, edit, and create files on your PC |
| `terminal-use` | Run and test code in the terminal (with safety restrictions) |

---

## Prerequisites

- [LM Studio](https://lmstudio.ai/) installed
- [Node.js](https://nodejs.org/) installed (for `npx`)
- A free [Exa API key](https://exa.ai/) (for the web search tool only)

---

## Setup

1. Open LM Studio and navigate to your `mcp.json` file
2. Choose which tools you want from the files in this repo
3. Copy the content into your `mcp.json`
4. Restart LM Studio

If you want all three tools at once, use `full-mcp-config.json` as a reference.

---

## Files

| File | Description |
|---|---|
| `exa-web-search.json` | Web search tool config |
| `file-access.json` | File read/write/create tool config |
| `terminal-use.json` | Terminal access tool config (with safety restrictions) |
| `full-mcp-config.json` | All three tools combined in one file |

---

## Notes

- For `file-access`, replace the placeholder path with the folder you want the LLM to access
- For `exa`, replace the placeholder with your own Exa API key — never share your real key publicly
- `terminal-use` comes with whitelisted commands and blocked system paths by default — edit carefully

---

## Author

Mohamed Ahmed — First-year CS student at FCAI, Cairo University.

[LinkedIn](https://www.linkedin.com/in/mohamed-ahmed-031266221?utm_source=share_via&utm_content=profile&utm_medium=member_android)
