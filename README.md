# ModelContextProtocol
Using MCP to connect to my stock broking account

Using Claude to connect to my Kite-Zerodha account via MCP
1. Install the claude desktop
2. Enable the MCP plugin settings for Kite inside Claude via Settings-> Developer -> EditConfig. Update the config with below snippet & save.
  ```
    "mcpServers": {
        "kite": {
            "command": "npx",
            "args": ["mcp-remote", "https://mcp.kite.trade/sse"]
        }
    }
 ```
3. Restart Claude desktop & authenticate to Kite.
4. Upon successful authentication be able to view & query data from Kite account into Claude

I have also performed some portfolio queries which are attached: Portfolio_query1.png & Portfolio_query2.png
