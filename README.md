# I build the runtime layer agents run on

I work on repo-scoped hooks, verification gates, lifecycle reminders, and local analytics for AI coding agents. The center of gravity is practical infrastructure for Claude Code, Codex CLI, and GitHub Copilot CLI: tools that make agent work easier to trust in real repositories.

## Current focus

- Agent hook runtimes that work across shells, operating systems, and coding-agent clients.
- Verification loops that turn "the agent says it is done" into something the machine checks.
- Local-first analytics and guardrails for developers who already use AI coding tools heavily.

## Projects

| Project | What it is for | Start here |
| --- | --- | --- |
| [lattice](https://github.com/LZong-tw/lattice) | Repo-scoped AI client hook runtime for Claude Code, Codex CLI, and GitHub Copilot CLI. Shared policy gates, lifecycle hooks, and provider integrations for real repos. | `pnpm add @lzong.tw/lattice` |
| [clawback](https://github.com/LZong-tw/clawback) | Verification loops for Claude Code and Codex: protected files, post-edit format/lint, stop-time typecheck, and context-compaction reminders. | `npx @lzong.tw/clawback` |
| [claude-code-usage-advisor](https://github.com/LZong-tw/claude-code-usage-advisor) | Read-only local analyzer for Claude Code history. It recommends practical model, effort, permission, sandbox, and prompt-cache profiles. | `npx claude-code-usage-advisor` |
| [pdf2epub-pro](https://github.com/LZong-tw/pdf2epub-pro) | High-fidelity PDF to EPUB pipeline with chunked parsing, restored PDF links, offline referenced-content appendices, and clean cover generation. | Clone and run from source |
| [readwise-reader-management](https://github.com/LZong-tw/readwise-reader-management) | Python scripts for Readwise Reader automation: tags, article operations, exports, and batch account maintenance. | Clone and configure locally |

## Live package signals

[![lattice npm downloads](https://img.shields.io/npm/dw/@lzong.tw/lattice?label=lattice%20downloads)](https://www.npmjs.com/package/@lzong.tw/lattice)
[![clawback npm downloads](https://img.shields.io/npm/dw/@lzong.tw/clawback?label=clawback%20downloads)](https://www.npmjs.com/package/@lzong.tw/clawback)
[![usage advisor npm downloads](https://img.shields.io/npm/dw/claude-code-usage-advisor?label=usage%20advisor%20downloads)](https://www.npmjs.com/package/claude-code-usage-advisor)

If one of these tools saves you a debugging session, a star on that repo tells me which experiments are worth keeping alive.

## What I am not trying to do

I do not want AI-generated volume, drive-by PR noise, or generic personal branding. The useful work is the shipped tool, the repro, the release note, and the issue that documents a real failure mode.
