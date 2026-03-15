# Fill Out Your Bracket

Use the shared Bracket Madness references instead of redefining the workflow here.

## Inputs

- Check `$ARGUMENTS` for `auto`.
- If `auto` is present, skip the strategy prompt and use autonomous bracket selection.

## Required references

1. Read `../../.codex/skills/bracketmadness/references/state.md`.
2. Read the `Fill` section in `../../.codex/skills/bracketmadness/references/workflows.md`.

## Execution notes

- Resolve keys using the shared state order.
- Use exact team names from `/api/bracket`.
- Preserve cross-round consistency across all 63 picks.
- Ask for confirmation before submission unless running in `auto` mode.
