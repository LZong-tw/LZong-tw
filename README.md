# Verification and inspection tools for AI coding agents

I work the operator side of Claude Code, Codex CLI, and GitHub Copilot CLI: hooks that stop agents from claiming "done" before code is checked, diagnostics that show what is really in the context window, and independent notes on how these tools behave at runtime.

Everything here is independent, version-pinned when behavior can drift, and built around reproducible evidence.

## Start Here

| Project | What it proves | Start here |
| --- | --- | --- |
| [clawback](https://github.com/LZong-tw/clawback) | Stop-time verification hooks for Claude Code and Codex: protected files, post-edit checks, typecheck/lint before "done", and compaction reminders. | `npx @lzong.tw/clawback` |
| [claude-code-field-notes](https://github.com/LZong-tw/claude-code-field-notes) | Independent, version-pinned notes on Claude Code runtime behavior: context, models, hooks, permissions, telemetry, transcripts, and settings. | Read the map |
| [ctxray](https://github.com/LZong-tw/ctxray) | Local-first inspection for agent context and routing: what was sent, why it routed that way, and where the context budget went. | `node src/cli/ctxray.mjs help` |
| [lattice](https://github.com/LZong-tw/lattice) | Repo-scoped hook dispatcher and policy layer for Claude Code, Codex CLI, and GitHub Copilot CLI. | `pnpm add @lzong.tw/lattice` |
| [claude-code-usage-advisor](https://github.com/LZong-tw/claude-code-usage-advisor) | Read-only inspection of Claude Code history, with practical recommendations for model, effort, permission, sandbox, and cache settings. | `npx claude-code-usage-advisor` |
| [readwise-reader-management](https://github.com/LZong-tw/readwise-reader-management) | Off-topic and older than the AI-agent tools, but it has the clearest public signal here: real stars and forks, no marketing. | Clone and configure locally |

## Operating Rules

- I do not treat npm downloads, clone counts, or badge numbers as adoption proof.
- I prefer small reproducible artifacts: a failing hook transcript, a version-pinned runtime note, a test that blocks the bad path, or an issue that documents a real failure mode.
- I do not want AI-generated volume, drive-by PR noise, or generic personal branding. The useful work is the shipped tool, the repro, the release note, and the field note that survives being checked by someone who knows the system.