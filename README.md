# EngageBay MCP for Cursor

Connect [Cursor](https://cursor.com) to your **EngageBay CRM** over the Model Context Protocol (MCP).

The agent can search and update contacts, companies, deals, notes, tags, and more — using your real EngageBay account data while you build.

## MCP server

| | |
|---|---|
| **URL** | `https://mcp.engagebay.com/mcp` |
| **Transport** | Streamable HTTPS |
| **Auth** | EngageBay OAuth (sign in when Cursor connects) |

This repo is the **public install config** for Cursor. The hosted MCP server runs at EngageBay; you do not run a local server.

## Requirements

- A **paid EngageBay** account
- [Cursor](https://cursor.com)
- Ability to complete EngageBay OAuth in the browser

## Install in Cursor

### Option A — from this config

1. Open **Cursor Settings → MCP** (or Features → MCP).
2. Add a server using the URL below, or merge the contents of [`.mcp.json`](./.mcp.json) into your Cursor MCP config:

```json
{
  "mcpServers": {
    "engagebay": {
      "url": "https://mcp.engagebay.com/mcp"
    }
  }
}
```

3. Enable **EngageBay** and complete OAuth when prompted.
4. In Agent chat, ask something like: *Find contacts tagged webinar from the last 30 days.*

### Option B — one-click (after directory listing)

Once published on [cursor.directory](https://cursor.directory), install from the EngageBay listing.

## What you can do

**Read:** search/get contacts, companies, deals, tasks, appointments; list properties, pipelines, tags, users; count records; read notes.

**Write:** create/update CRM records; add notes; manage tags and associations; set owners.

Access follows the scopes you approve at sign-in. Claude/Cursor will ask before write tools when annotations require it.

## Docs

- Product / setup (Claude guide also covers the same MCP URL): [EngageBay for Claude](https://www.engagebay.com/product/mcp/cursor)
- Privacy: [Privacy Policy](https://www.engagebay.com/legal/privacy-policy)
- Terms: [Terms of Service](https://www.engagebay.com/legal/terms-of-service)
- Website: [engagebay.com](https://www.engagebay.com)

## Support

- Email: support@engagebay.com  
- Integrations: integrations@engagebay.com  

## License

Docs and config in this repository are provided by EngageBay Inc. for connecting to the EngageBay MCP service.
