# CLAUDE.md — subagentplugins org

Guidance for Claude when working anywhere in the `subagentplugins` org. Internal-facing.

## Scope of this file

This lives in the org's `.github` repo and is the canonical agent-guidance file for **org-level** concerns. It does **not** auto-load into other repos — clone each repo on its own and follow that repo's `CLAUDE.md` first; fall back to this file only for cross-repo conventions.

## What this org is

The plugins / connectors / MCP surface for the `subagentmcp` enterprise. Repo index lives in [README.md](README.md) of this repo.

Sister org: [`subagentapps`](https://github.com/subagentapps) (products and apps).

## Org-level conventions

- **Default branch:** `main`. Force-push disabled. PRs require review.
- **Repo's own files win.** A repo's `CLAUDE.md`, `AGENTS.md`, or `README.md` overrides anything here.
- **Polyrepo orchestrator:** `subagenttypescript` is the worktree-based multi-repo runtime for this org. For cross-repo work, start there.
- **Marketplace forks** (`claude-plugins-official`, `claude-plugins-community`, `knowledge-work-plugins`, `financial-services-plugins`) are upstream mirrors — only modify if the user explicitly asks. Submissions to upstream marketplaces go through their published submission flows, not by editing the fork.
- **Profile README is aspirational.** [profile/README.md](profile/README.md) names repo-prefix conventions (`plugin-*`, `connector-*`, `mcp-*`) and a `manifest.yaml + prompt + eval` shape that the current repo set does not actually follow. Don't treat it as ground truth.

## Identity

The user has multiple GitHub aliases (admin-jadecli, alex-jadecli, jade-jadecli, jane-jadecli, gemma-jadecli) — all the same human. Don't flag this as account confusion. If unsure which alias to commit/push as, ask.

## When something is unclear

Ask before:
- Pushing to `main` directly.
- Modifying any of the marketplace forks.
- Cross-repo refactors that span more than one repo in this index — coordinate via `subagenttypescript`.
