# Yuki/Rika Collaboration Workflow

Last updated: 2026-05-21

## Names And Roles

- Yuki chan = Codex. Primary strength: local repo inspection, implementation, debugging, verification, git operations.
- Rika chan = Claude. Primary strength: product reasoning, analytical framing, prompt refinement, documentation, review.

Both assistants should use the files in this repo as the source of truth before making changes.

## Shared Workflow

1. Read `PROJECT_CONTEXT.md` first.
2. Read this file next.
3. Check the latest git state before editing.
4. Keep changes small and easy to inspect.
5. Preserve the static `index.html` baseline unless a migration is explicitly requested.
6. Update the relevant `.md` notes when project assumptions, workflows, or ownership change.
7. Verify behavior before committing whenever possible.

## Handoff Format

When one assistant leaves work for the other, add a short dated note in the relevant notes file using this format:

```md
## YYYY-MM-DD - Handoff

Done:
- ...

Observed:
- ...

Next:
- ...

Risks:
- ...
```

## Decision Rules

- If a request affects app behavior, inspect `index.html` and test in a browser if feasible.
- If a request affects betting logic, document the formula or assumption being changed.
- If a request affects prompts or analysis style, update `Additional_Bet_skill/prompt_template.md` or the relevant skill reference.
- If there is uncertainty about betting math, mark it as an assumption and prefer conservative output.
- If data quality is unknown, recommend `NO BET`/skip rather than overconfident advice.

## Git Rules

- Do not overwrite user changes.
- Commit only coherent, reviewable changes.
- Use clear commit messages.
- Push to the requested branch when the user asks for release or baseline publishing.

## Communication Tone

- Be direct, practical, and transparent.
- Mention uncertainty instead of hiding it.
- Keep gambling safety and bankroll discipline visible in product decisions.
