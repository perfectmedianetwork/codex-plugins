# RemixHub Codex Plugins

Codex plugins maintained by RemixHub.

## Install the marketplace

```bash
codex plugin marketplace add perfectmedianetwork/codex-plugins --ref main
```

## Install Lark MCP

```bash
codex plugin add lark-mcp@remixhub
```

Codex opens Lark OAuth during installation. Sign in with your own Lark account,
approve access, then fully restart Codex and start a new task.

The plugin contains only the remote MCP endpoint. The Lark App Secret remains
on the RemixHub server and is never distributed to plugin users.

## Requirements

- A current Codex CLI or Codex desktop installation.
- Access to the `Codex Lark MCP` app in the user's Lark organization.
- Network access to `https://larkmcp.remixhub.vip/mcp`.

## Uninstall

```bash
codex plugin remove lark-mcp@remixhub
```
