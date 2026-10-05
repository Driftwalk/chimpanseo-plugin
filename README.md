# ChimpanSEO plugin for Cursor

Write, refresh, publish and schedule SEO/GEO-optimized articles on your WordPress site without leaving Cursor.

[ChimpanSEO](https://chimpanseo.app) writes articles structured so that Google and AI search engines can cite them, and publishes them through the WordPress REST API. This plugin connects Cursor to the ChimpanSEO remote MCP server and adds a skill that walks the agent through the workflow.

## What's inside

- `mcp.json`: the remote MCP server (`https://chimpanseo.app/api/mcp`, Streamable HTTP)
- `skills/chimpanseo-articles`: how to plan, generate, review and publish articles with the 13 tools

## Setup

1. Create a ChimpanSEO account (15-day free trial) and connect your site.
2. In the dashboard, open Settings > API/MCP and create an API key.
3. Set it as an environment variable before starting Cursor:

```bash
export CHIMPANSEO_API_KEY="csk_..."
```

Then ask the agent, for example: "Suggest five topics for my site and write the first one as a draft."

## Tools

`list_sites`, `get_usage`, `list_articles`, `get_article`, `suggest_topics`, `list_scheduled_articles`, `audit_site`, `get_generation_status`, `generate_article`, `refresh_article`, `publish_article`, `schedule_article`, `cancel_scheduled_article`.

Full documentation: https://chimpanseo.app/mcp

## Pricing

The MCP server is included in every ChimpanSEO plan. After the trial: Starter EUR 19/month, Pro EUR 59/month (scheduling included), Business EUR 149/month.

## License

MIT
