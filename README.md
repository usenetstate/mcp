# Netstate MCP

Search 128 million official company registrations across every US state, DC, Puerto Rico and Canada.

This repository is a public listing for the Netstate MCP server. The server itself runs remotely — this repo does **not** contain the production site source, only the metadata files used by MCP directories.

- **Website:** [https://netstate.co](https://netstate.co)
- **Remote endpoint:** `https://netstate.co/mcp`
- **Transport:** Streamable HTTP (stateless, no authentication required)
- **Official Registry name:** `co.netstate/netstate`
- **Privacy policy:** [https://netstate.co/privacy](https://netstate.co/privacy)
- **License:** MIT

## Tools

| Tool | Description |
| --- | --- |
| `search_companies` | Search official company registrations by name across all supported jurisdictions. |
| `list_jurisdictions` | List every supported jurisdiction (all US states, DC, Puerto Rico and Canada). |
| `get_site_info` | Get information about the Netstate service and its data coverage. |

## Usage

Netstate MCP is a remote server. There is nothing to install or run locally — just point your MCP client at the endpoint. No API key or secrets are needed.

### Cursor / Claude (`mcp.json`)

```json
{
  "mcpServers": {
    "netstate": {
      "url": "https://netstate.co/mcp"
    }
  }
}
```

In Cursor, add this to `.cursor/mcp.json` (project) or `~/.cursor/mcp.json` (global). In Claude Desktop or other MCP clients that support remote servers, use the same URL with the Streamable HTTP transport.

## License

[MIT](LICENSE) © Netstate 2026
