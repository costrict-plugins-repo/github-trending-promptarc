# promptarc plugin for Claude Code

> Session intelligence for AI coding agents. Get AI briefings, generate PR descriptions, share sessions, and search your history — inside Claude Code.

## Install

```
/plugin marketplace add promptarc/promptarc-plugin
/plugin install promptarc@promptarc/promptarc-plugin
```

## Commands

```
/promptarc:context     AI briefing: what's unfinished, resume prompt, warnings
/promptarc:pr          Generate a PR description from this session
/promptarc:share       Share this session to the cloud (private, redacted)
/promptarc:search      Search past sessions in your cloud archive
```

## What it does

- **`/promptarc:context`** — Scans local sessions + cloud archive, generates an AI briefing with what's unfinished, a copy-pasteable resume prompt for your agent, and warnings from past failures. Works across Claude Code, Codex, and Cursor sessions.
- **`/promptarc:pr`** — Generates structured PR descriptions (What / Why / How / Notes) from the current session. Pipe to `gh pr create` for zero-copy workflow.
- **`/promptarc:share`** — Shares a session to the cloud. Builds the artifact locally, redacts secrets before upload. Auto-signs in if needed.
- **`/promptarc:search`** — Searches across every message, tool call, file path, and error in your cloud archive.

## Requirements

- Claude Code
- `promptarc` CLI (`npm i -g promptarc`) or commands auto-install via `npx`

## Privacy

- Secrets are redacted **locally** before any upload
- Shares default to **private**
- Only condensed summaries (~2K tokens) are sent for AI features — no code content

## Links

- [promptarc.dev](https://promptarc.dev)
- [npm package](https://www.npmjs.com/package/promptarc)
- [Feedback](https://promptarc.dev/feedback)
