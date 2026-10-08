# Lark MCP for Codex

This plugin connects Codex to the RemixHub-hosted Lark MCP endpoint:

`https://larkmcp.remixhub.vip/mcp`

On installation, Codex opens Lark OAuth. Each user signs in with their own Lark
account, so tool calls use that user's Lark permissions. The Lark App Secret is
never distributed with the plugin and remains stored as a Docker secret on the
server.

Available tool groups include Lark messaging, Base, documents, wiki, contacts,
Drive permissions, task create/read/update/delete operations, follower
management, and shared tasklist creation/membership/listing operations.

The company-directory tools are read-only and cover listing child departments,
reading one department, listing a department's direct members, and reading one
user's basic profile. The plugin does not expose contact create, update, or
delete operations. Results remain limited by each signed-in user's Lark data
visibility.

Lark does not expose a tenant-wide administrator override for all standalone
tasks. For a company-wide view, use a shared tasklist, grant the company group
or relevant employees access, and add company tasks to that list. The MCP can
then enumerate the list and its tasks with the caller's own Lark permissions.

Users must be included in the Lark application's availability scope before they
can authorize the plugin.
