# Gregale plugin for Antigravity

Deploy, diagnose and roll back Gregale apps from Antigravity. The plugin adds:

- Gregale's hosted MCP server (`https://api.gregale.dev/mcp`) via
  [`mcp_config.json`](./mcp_config.json). The first time Antigravity connects,
  sign in to Gregale (or sign up), choose what the agent may do and which apps
  it may use, and connect;
- the `deploy` skill, which deploys the current project, verifies an application
  response and rolls back a broken release with your approval;
- the `diagnose` skill, which finds why an app is failing or slow from health,
  error groups, logs, and request timelines;
- `rules/AGENTS.md` with the safe operational defaults both skills follow.

## Install

Install from Antigravity via the Plugin Manager by pointing to this repository,
or run `agy plugin install https://github.com/gregale-dev/gregale-antigravity-plugin`.

The skills can also deploy with the `gregale` CLI; install it and log in (or set
`GREGALE_TOKEN`): https://gregale.dev/docs/install

## Links

- [Antigravity & MCP setup docs](https://gregale.dev/docs/antigravity)
- [Deploy from Antigravity IDE guide](https://gregale.dev/articles/antigravity-ide-mcp-server-deploy)
- [Gregale agent guide](https://gregale.dev/docs/agents)
- [CLI & MCP setup](https://gregale.dev/docs/cli)

## License

Apache-2.0 — see [LICENSE](./LICENSE).
