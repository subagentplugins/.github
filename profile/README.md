# subagentplugins

Welcome to **subagentplugins** — the plugins surface of the [`subagentmcp`](https://github.com/enterprises/subagentmcp) enterprise. This org hosts knowledge-work plugins, connectors, and MCP servers used by Claude Cowork as an autonomous orchestrator across enterprise departments.

## What lives here

- **Plugins** — knowledge-work plugins for Claude Cowork (skills, runbooks, workflow recordings).
- **Connectors** — integration shims for SaaS surfaces (Gmail, Drive, Slack, GitHub, Linear, etc.).
- **MCPs** — Model Context Protocol servers exposing internal systems to Claude.
- **`.github`** — org-wide profile, contribution guide, and shared GitHub Actions workflows.

## How it fits together

```
Claude Cowork (orchestrator)
  └─ Connectors / MCPs (this org)
       └─ Skills directory (department / skill-name)
            └─ Plugins (this org)
```

Claude Cowork plans → user approves → Claude executes via Claude in Chrome, calling skills published from this org.

## Conventions

- Repos are prefixed by surface: `plugin-*`, `connector-*`, `mcp-*`.
- Each plugin ships a `manifest.yaml`, a prompt, and a small held-out eval set.
- Default branch: `main`. PRs require review; force-push is disabled.
- Security: Dependabot alerts + version updates on, secret scanning on, code scanning default setup on.

## Related orgs

- [`subagentapps`](https://github.com/subagentapps) — application code and product surfaces.
- Enterprise root: [`subagentmcp`](https://github.com/enterprises/subagentmcp).

## Getting started

1. Browse repositories in this org.
2. Read the relevant plugin's `README.md` and `manifest.yaml`.
3. File issues against the specific plugin repo; cross-cutting issues go in `.github`.
