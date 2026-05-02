# subagentplugins/.github

Internal index for the `subagentplugins` GitHub org. Public org-page content lives in [profile/README.md](profile/README.md); this file is for engineers and agents working across the org.

The org is the **plugins / connectors / MCP** surface of the [`subagentmcp`](https://github.com/enterprises/subagentmcp) enterprise. Sister org for products/apps: [`subagentapps`](https://github.com/subagentapps).

## Repositories

Authoritative state: `gh repo list subagentplugins --limit 100`. Per-repo conventions live in each repo's own README — this index points, it does not document.

### First-party

- [subagenttypescript](https://github.com/subagentplugins/subagenttypescript) — polyrepo orchestrator (TypeScript) for this org. Worktree-based multi-repo agent runtime.
- [subagentcoworkers](https://github.com/subagentplugins/subagentcoworkers) — TypeScript.
- [subagentroutines](https://github.com/subagentplugins/subagentroutines) — scheduled / recurring routines.

### Plugin marketplaces (forks)

- [claude-plugins-official](https://github.com/subagentplugins/claude-plugins-official) — fork of Anthropic's official Claude Code plugins directory (Python).
- [claude-plugins-community](https://github.com/subagentplugins/claude-plugins-community) — fork of the community plugin marketplace for Claude Cowork & Claude Code. Read-only mirror; submit upstream at `clau.de/plugin-directory-submission`.
- [knowledge-work-plugins](https://github.com/subagentplugins/knowledge-work-plugins) — fork of the knowledge-worker plugin set (Python).
- [financial-services-plugins](https://github.com/subagentplugins/financial-services-plugins) — fork (Python).

### Org infrastructure

- [.github](https://github.com/subagentplugins/.github) — this repo. Public org profile + shared workflows (e.g., `auto-assign-issues`).

## Working in this org

- Default branch: `main`. PRs require review; force-push disabled.
- Identity aliases: see your global `~/.claude/CLAUDE.md` (admin-jadecli, alex-jadecli, jade-jadecli, jane-jadecli, gemma-jadecli — all the same human).
- The polyrepo orchestrator for this org is `subagenttypescript` — for cross-repo work, start there.
- Per-repo guidance lives in each repo's `README.md` / `CLAUDE.md` / `AGENTS.md`. Files in this repo do **not** auto-propagate to other repos.

## Note on the public profile

[profile/README.md](profile/README.md) describes aspirational repo-prefix conventions (`plugin-*`, `connector-*`, `mcp-*`) and a `manifest.yaml + prompt + eval` layout. Those conventions are **not currently enforced** — the actual repo set above is mostly forks and a TypeScript orchestrator. Treat the profile as marketing, not as ground truth.

## Agent guidance

See [CLAUDE.md](CLAUDE.md) and [AGENTS.md](AGENTS.md).
