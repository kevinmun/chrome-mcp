### Setup Chrome Remote Debugging

1. Close Chrome completely
2. Launch Chrome with remote debugging enabled:

```bash
/Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome --remote-debugging-port=9222 --user-data-dir=data/.chrome-debug-profile
```

### Load MCP Server in Cursor

After starting Chrome with remote debugging:

**Reload MCP Servers (Preferred)**
1. Open Cursor Settings (`Cmd+,`)
2. Navigate to **MCP** section
3. Find the `browser` server and click the **Refresh** button (↻)

### Verify Connection

Check that the MCP browser server is connected:
- In **Settings > MCP**, the browser server should show a green status
- Test by running `curl http://127.0.0.1:9222/json` — should return JSON with open tabs

### Usage

Query the data via Cursor Ask/Plan/Agent Mode

