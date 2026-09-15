# Grok Bot (Agent Plugins) packaging

This fork packages ZoomInfo's hosted MCP server and skills for the Grok Bot Agent Plugins marketplace.

## Compatibility

- **Root `plugin.json`** — Agent Plugins schema (`agent-plugins.org`) metadata for Grok Bot.
- **Root `mcp.json`** — streamable HTTP to `https://mcp.zoominfo.com/mcp` (OAuth handled by the hosted MCP; no API keys in-repo).
- **`skills/`** — task-focused playbooks (unchanged from upstream).
- **Cursor** — use `mcp.cursor.json` (`mcp-remote` OAuth bridge) and `.cursor-plugin/`.
- **Claude / Codex** — use `.mcp.json` and the nested `.claude-plugin/` / `.codex-plugin/` manifests.

Do not add hooks, rules, agents, or commands for this packaging path.

## Submit for marketplace review

1. Ensure this repository is public (open source).
2. Submit at **https://cursor.com/marketplace/publish** for manual review.
3. **Do not** submit via `https://github.com/xai-org/plugin-marketplace`.

## Attribution

Upstream product and branding: [ZoomInfo](https://www.zoominfo.com). This repository is a fork under [CloudNerdATX](https://github.com/CloudNerdATX/zoominfo-mcp-plugin) focused on Grok Bot Agent Plugins packaging.
