# Lark MCP for Codex

This plugin connects Codex to the RemixHub-hosted Lark MCP endpoint:

`https://larkmcp.remixhub.vip/mcp`

On installation, Codex opens Lark OAuth. Each user signs in with their own Lark
account, so tool calls use that user's Lark permissions. The Lark App Secret is
never distributed with the plugin and remains stored as a Docker secret on the
server.

Available tool groups include Lark messaging, Base, documents, wiki, contacts,
Drive permissions, and task create/read/update/delete operations.

Users must be included in the Lark application's availability scope before they
can authorize the plugin.
