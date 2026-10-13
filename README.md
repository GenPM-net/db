# @core/db

[![genpm](https://api.genpm.net/v1/badge/@core/db.svg)](https://genpm.net/p/@core/db) ![license](https://img.shields.io/badge/license-MIT-blue)

> Postgres with Drizzle: shared client, per-module schemas, transactions and ULID ids

A [GenPM](https://genpm.net) module: **source code + AI rules + MCP config**, injected into your project instead of hidden in `node_modules`. The code lands in `src/lib/db`, pinned to a verified commit, and you own it.

## Install

```bash
genpm add @core/db
```

No genpm yet? `curl -fsSL https://genpm.net/install.sh | sh` (macOS/Linux), `irm https://genpm.net/install.ps1 | iex` (Windows), or one-off with `npx @genpm-net/cli add @core/db`.

Or let your AI agent do it: run `genpm mcp setup` once, then ask *"add @core/db with genpm"* in Claude Code, Cursor, VS Code, Windsurf, Codex or Gemini CLI. It shows you a dry-run plan before writing anything.

## What it does

Shared Postgres access for every module: one Drizzle client, per-module schemas, transactions, ULID ids and standard
timestamps. It owns no tables itself. Not an ORM wrapper: use Drizzle's query builder directly.

## At a glance

- **npm dependencies** (proposed, never installed without asking): `drizzle-orm`, `postgres`
- **Environment variables** (added to `.env.example`): `DATABASE_URL`
- **AI rules**: [`AGENTS.md`](AGENTS.md), loaded by your agent only when it works in `src/lib/db`

## Security

GenPM installs a 40-character commit SHA (never a branch), verifies an Ed25519-signed manifest, never runs install scripts and scans AI rules for prompt injection. Details: [genpm.net/docs/security](https://genpm.net/docs/security).

## License

MIT — see [LICENSE](LICENSE). Browse the full catalog at [genpm.net](https://genpm.net).
