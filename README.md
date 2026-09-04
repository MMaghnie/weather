# Demo MCP Server setup

Mainly following the official tutorial from Anthropic:
[Build an MCP server](https://modelcontextprotocol.io/docs/2026-07-28/develop/build-server) (*)

## (*) Implementation Notes:

After building & running the MCP server, when you're about to test it with Claude Desktop, the tutorial specifies the need to create a config file `claude_desktop_config.json` ([Testing your server with Claude for Desktop](https://modelcontextprotocol.io/docs/2026-07-28/develop/build-server#testing-your-server-with-claude-for-desktop)) at `AppData\Claude\claude_desktop_config.json`.

But this path may be incompatible with the actual Claude Desktop installation on your MradServices PC. 

### How to open the file automatically on your system:
1. Open the **Claude Desktop** app.
1. Go to the system tray menu and open **Settings**.
1. Click on the *Developer* tab on the left sidebar.
1. Click the **Edit Config** button to open or create the file automatically.

Then add the `mcpServers` schema to the file, save the changes, and restart **Claude Desktop**.

You can then pick up with the instructions from the official tutorial at this step: [Test with commands](https://modelcontextprotocol.io/docs/2026-07-28/develop/build-server#test-with-commands)