# Runner in the MCP Registry

[Runner](https://www.runtheworld.ai): they run the work, you run the world. Your runners, in one app: they do your marketing and keep every deal moving, inside the limits you set.

This repository holds Runner's entry in the [official MCP Registry](https://registry.modelcontextprotocol.io) as `io.github.runtheworldai/runner`. Runner's MCP server is hosted, so there is nothing to install:

```
https://app.runtheworld.ai/api/mcp
```

Sign-in is OAuth with your own Runner account. Setup for Claude, Claude Code and ChatGPT: [Use Runner in Claude and ChatGPT](https://www.runtheworld.ai/guides/use-runner-in-claude-and-chatgpt).

## Publishing

`server.json` is published by `.github/workflows/publish-mcp.yml` through GitHub OIDC, so no registry token is stored anywhere. Change `server.json`, bump `version`, push to `main`, and the workflow publishes the new version. It can also be run by hand from the Actions tab.

Questions: team@runtheworld.ai
