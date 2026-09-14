# Model Context Protocol (MCP) Server Integration Guide

This guide details how to securely connect an autonomous AI agent to local and cloud systems using the Model Context Protocol (MCP).

## ⚙️ Core Configuration Archetypes

### Local Filesystem Access Server
```json
{
  "mcpServers": {
    "filesystem": {
      "command": "npx",
      "args": [
        "-y",
        "@modelcontextprotocol/server-filesystem",
        "/path/to/allowed/sandbox/directory"
      ]
    }
  }
}
```

### Secure Local Credential Broker
```json
{
  "mcpServers": {
    "secure-broker": {
      "command": "node",
      "path": "/usr/local/bin/mcp-credential-broker.js",
      "env": {
        "ENCRYPTION_KEY": "via-system-environment-variable-only"
      }
    }
  }
}
```
