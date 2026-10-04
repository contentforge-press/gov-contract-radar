# GovContract Radar

![npm](https://img.shields.io/npm/v/gov-contract-radar-mcp)
![npm downloads](https://img.shields.io/npm/dm/gov-contract-radar-mcp)

**AI-native MCP server for U.S. federal contract opportunities (SAM.gov).**
Filter new federal solicitations by NAICS code and set-aside status (8(a), SDVOSB, WOSB, HUBZone), get deadlines and agency details — delivered the day they post.

Built on public U.S. government data (SAM.gov, USAspending). No login walls, no scraping of private data.

## Highlights

- **Live opportunities**: new SAM.gov solicitations filtered by your NAICS codes
- **Set-aside filtering**: 8(a), SDVOSB, WOSB, HUBZone flags on every opportunity
- **Deadline-first**: response deadlines surfaced on every card
- **Email alerts**: daily digest of new matches (optional subscription)
- **MCP-native**: connect Claude, Cursor or any MCP client

## Connect

**Streamable HTTP endpoint:** `https://gov.pixharvest.com/mcp`

```json
{
  "mcpServers": {
    "gov-contract-radar": {
      "type": "streamable-http",
      "url": "https://gov.pixharvest.com/mcp"
    }
  }
}
```

## Tools

| Tool | Description |
|---|---|
| `search_opportunities` | Query federal contract opportunities by NAICS, keyword or set-aside |
| `get_opportunity` | Full detail for a specific solicitation |

## Pricing

| Plan | Price | Includes |
|---|---|---|
| Starter | $19/mo | NAICS filtering, daily digest, 7-day free trial |
| Pro | $49/mo | Everything + set-aside alerts + more matches |
| Radar+ | $149/mo | Priority data, custom filters, team access |

Pay by card or bank transfer (invoice). No card required for the free trial.

## Website

- Product: https://pixharvest.com/gov
- Pay by invoice: https://pixharvest.com/pay
- MCP directory page: https://glama.ai/mcp/connectors/com.pixharvest/gov-contract-radar

## License

MIT
