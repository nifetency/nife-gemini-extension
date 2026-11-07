# Nife extension for Gemini CLI

Connects Gemini CLI to the hosted Nife MCP server at `https://mcp.on.nifetency.com/mcp`, so you can deploy and manage your Nife.io sites from the terminal: deploy from a Git repository or source, check status, releases, analytics and bandwidth, and manage custom domains and Git secrets.

Disclosure: I'm the founder of Nife.

## Install

```bash
gemini extensions install https://github.com/nifetency/nife-gemini-extension
```

## Sign in

The first time a Nife tool is used, Gemini CLI opens a browser window. Log in with your Nife account at launch.nife.io and approve access (scope: `mcp`). Gemini CLI stores the token locally. If it asks for it, run `/mcp auth nife`.

You need a Nife account. Sign up at https://nife.io.

## Tools

The server exposes 25 tools. Each tool declares whether it is read-only, changes data or is destructive (for example, deleting a site). Run `/mcp` in Gemini CLI to list them.

Note: the Git secret tool takes a personal access token as an argument. Use a token with the minimum scope you need.

## Links

- Server source: https://github.com/nifetency/nife-mcp-server
- Privacy policy: https://nife.io/privacy
- Support: nida@nife.io

## License

MIT
