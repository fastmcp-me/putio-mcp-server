[![Add to Cursor](https://fastmcp.me/badges/cursor_dark.svg)](https://fastmcp.me/MCP/Details/1082/putio)
[![Add to VS Code](https://fastmcp.me/badges/vscode_dark.svg)](https://fastmcp.me/MCP/Details/1082/putio)
[![Add to Claude](https://fastmcp.me/badges/claude_dark.svg)](https://fastmcp.me/MCP/Details/1082/putio)
[![Add to ChatGPT](https://fastmcp.me/badges/chatgpt_dark.svg)](https://fastmcp.me/MCP/Details/1082/putio)
[![Add to Codex](https://fastmcp.me/badges/codex_dark.svg)](https://fastmcp.me/MCP/Details/1082/putio)
[![Add to Gemini](https://fastmcp.me/badges/gemini_dark.svg)](https://fastmcp.me/MCP/Details/1082/putio)

# putio-mcp-server
MCP server for interacting with put.io

## Features

- List active transfers
- Add new transfers via URL or magnet link
- Cancel existing transfers
- Get browser links for completed transfers

## Prerequisites

- [Claude Desktop](https://modelcontextprotocol.io/quickstart/user)
- Python 3.x
- [uvx](https://docs.astral.sh/uv/getting-started/installation/)
- Put.io account and API token ([guide](https://help.put.io/en/articles/5972538-how-to-get-an-oauth-token-from-put-io))

## Setup

Put following config in your `claude_desktop_config.json`.

Don't forget to replace `<your-putio-api-token>` with your own API token.


```json
{
  "mcpServers": {
    "putio": {
      "command": "uvx",
      "args": [
        "putio-mcp-server"
      ],
      "env": {
        "PUTIO_TOKEN": "<your-putio-api-token>"
      }
    }
  }
}
```
