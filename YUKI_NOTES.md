# Yuki Notes

Last updated: 2026-05-21

## Operating Picture

This repo is a static football betting assistant. The current baseline is intentionally simple: no build system, no dependencies, and no backend. `index.html` should open directly in a browser and remain useful offline except for any future data integrations.

## What I Checked

- Project folder contains one main app file and one `Additional_Bet_skill` folder.
- `index.html` includes calculator, history, and stats tabs.
- Local history uses `localStorage` key `hutao_bets`.
- Strategy docs cover football data checks, live betting discipline, market traps, multi-agent analysis, and prompt structure.
- The folder was not a Git repository at the start of this baseline pass.

## Implementation Preferences

- Keep future edits compatible with a static GitHub Pages deployment unless the user asks for a framework.
- Prefer focused changes inside `index.html` over creating scattered partial files.
- If app complexity grows, propose a light structure before splitting files.
- Add tests only when there is a real test harness or when moving logic out of inline script.

## Known Follow-ups

- Clean mojibake text while preserving the intended wording.
- Add a simple smoke-test checklist for manual browser verification.
- Consider extracting betting math into a separate JS module if the app grows.
- Add odds format conversion for MY/HK/decimal as requested in the roadmap.

## 2026-05-21 - Handoff

Done:
- Read current project files.
- Created shared context and assistant collaboration docs.

Observed:
- Static app baseline is understandable and useful.
- Encoding cleanup is the clearest low-risk polish item.

Next:
- Initialize/connect git and push baseline to the requested `Bet_assist_app` branch.

Risks:
- No automated tests exist yet.
- Betting formulas should be reviewed carefully before presenting future outputs as stronger recommendations.
