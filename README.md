# Telinfy Cursor Plugin

Cursor plugin for [Telinfy](https://telinfy.com): send consent-gated SMS and WhatsApp campaigns, manage phonebooks, and pull delivery reports from Cursor.

This repository contains only the plugin definition: a manifest, the remote MCP server address, a usage rule and a logo. The MCP server itself is hosted by Telinfy at `https://mcp.telinfy.com`; nothing runs locally.

See [plugins/telinfy/README.md](plugins/telinfy/README.md) for setup and the tool list, and https://mcp.telinfy.com/docs for full documentation.

## Layout

```
.cursor-plugin/marketplace.json        marketplace index
plugins/telinfy/.cursor-plugin/plugin.json
plugins/telinfy/mcp.json               remote MCP server (OAuth sign-in)
plugins/telinfy/rules/telinfy-messaging.mdc
plugins/telinfy/assets/logo.png
```

## Support

support@telinfy.com
