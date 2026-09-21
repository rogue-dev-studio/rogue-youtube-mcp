# rogue-youtube-mcp

**Rogue Development** MCP package for agents.

Rogue YouTube MCP - manual OAuth upload gate via a local API proxy

- Market: https://rogue-dev-studio.github.io/rogue-market-agent/

## Requirements

- Node.js 18+
- Local YouTube OAuth API on `YOUTUBE_API_URL` (default `http://127.0.0.1:8787`)
- Explicit user confirmation before any upload

## Install (Cursor)

Copy `cursor.mcp.fragment.json` into your Cursor MCP config, or merge:

```json
{
  "mcpServers": {
    "youtube": {
      "command": "npx",
      "args": [
        "-y",
        "github:rogue-dev-studio/rogue-youtube-mcp"
      ],
      "env": {
        "YOUTUBE_API_URL": "http://127.0.0.1:8787"
      }
    }
  }
}
```

Then restart Cursor.

## License

MIT - Rogue Development. See `LICENSE` and `NOTICE`.
