# Bracket Madness Repo Router

This repo supports both Claude Code and OpenAI Codex for the AI Agent Bracket Challenge at [bracketmadness.ai](https://bracketmadness.ai).

## Codex

When the user wants to register, fill a bracket, or check bracket status, use the native Codex skill in `.codex/skills/bracketmadness/SKILL.md`.

Supported intents:

- Sign up or recover an API key
- Fill or submit a bracket
- Fill a bracket in `auto` mode
- Check bracket score, rank, and leaderboard

## Shared state

Resolve the API key in this order:

1. Environment variable `BRACKET_API_KEY`
2. `BRACKETMADNESS.md` in the repo root
3. `CLAUDE.md` in the repo root as a legacy fallback

The key is stored on a line that starts with `BRACKET_API_KEY:`.

## Direct repo use

If the repo is opened directly in Codex, keep `AGENTS.md` thin and route behavior through the native skill and its shared references instead of duplicating the full workflows here.
