---
name: cesto-toolkit
description: Turn any coding agent into a full Cesto client — browse and analyze baskets, simulate portfolios against the S&P 500, and create baskets on Cesto Labs. Use when building on Cesto, exploring baskets, or embedding basket widgets.
metadata:
  version: 1.0.0
  homepage: https://docs.cesto.co/cesto/skill
  repository: https://github.com/cesto-co/cesto-skills
---

# Cesto Toolkit

The Cesto Toolkit is an open-source AI agent skill for [Cesto](https://cesto.co) — a platform for investing in narrative-driven baskets of assets on Solana. It works with any agent that supports skills: Claude Code, Cursor, Codex, Windsurf, and 60+ others.

## Install

```bash
npx skills add cesto-co/cesto-skills --skill cesto-toolkit
```

## What it does

- **Browse and analyze** every basket — names, categories, risk levels, allocations, token prices, market caps, volume, and historical returns. No login required.
- **Compare performance** across baskets and against the S&P 500 benchmark over time.
- **Simulate portfolios** — backtest any custom token allocation against the S&P 500 (both start at $1,000) with daily historical data.
- **Create baskets on Cesto Labs** — publish custom token allocations, vote on community baskets, and pull the creator leaderboard. Preview everything before it goes live.

## Authentication

Only basket creation and portfolio simulation require authentication. A magic-link flow opens your browser to connect a Solana wallet and sign a message; credentials are stored at `~/.cesto/auth.json` with restricted permissions and never printed in agent output. Browsing and analytics work without logging in.

## Related surfaces

- **Cesto SDK** (`@cesto/sdk`) — a typed, server-side TypeScript client for the read-only API (baskets and positions). See https://docs.cesto.co/sdk/overview.
- **Cesto Widgets** — embeddable, iframe-based basket cards for any website. See https://docs.cesto.co/widgets/overview.

## Learn more

- Skill docs: https://docs.cesto.co/cesto/skill
- Source: https://github.com/cesto-co/cesto-skills
