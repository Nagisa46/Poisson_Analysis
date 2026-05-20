# HuTao Bet Assistant App - Project Context

Last updated: 2026-05-21

## Product Summary

HuTao Bet Assistant is a static, mobile-first football betting decision assistant. The current app is delivered as a single `index.html` file and combines:

- Poisson match probability modeling.
- Dixon-Coles low-score correction.
- Weighted recent form adjustment.
- 1X2 implied probability and expected value comparison.
- Asian Handicap probability and EV support.
- Over/Under probability and EV support.
- Kelly stake sizing.
- Local browser bet history, result tracking, CLV tracking, and basic performance stats.

The app is meant to support disciplined betting decisions, not guarantee outcomes.

## Current File Map

- `index.html` - GitHub Pages launcher for choosing between app versions.
- `main-app/index.html` - Original `main` branch Poisson Pro app for Pages access.
- `bet-assist-app/index.html` - HuTao Bet Assistant app for Pages access.
- `HuTao_Bet_Assistant_App_RoadMap.txt` - Original roadmap, phases, pros/cons, risks, and recommendations.
- `Additional_Bet_skill/football_data_checklist.md` - Pre-bet data checklist.
- `Additional_Bet_skill/live_betting_skill.md` - Live betting decision guidance.
- `Additional_Bet_skill/market_trap_patterns.md` - Market trap reference.
- `Additional_Bet_skill/market_trap_patterns.txt` - Same market trap reference in `.txt` form.
- `Additional_Bet_skill/multi_agent_workflow.md` - Analyst role workflow.
- `Additional_Bet_skill/prompt_template.md` - Football analysis prompt template.
- `YUKI_RIKA_WORKFLOW.md` - Shared collaboration protocol for Yuki and Rika.
- `YUKI_NOTES.md` - Codex/Yuki operating notes.
- `RIKA_NOTES.md` - Claude/Rika operating notes.
- `PAGES_LINKS.md` - Stable GitHub Pages links and Pages settings.

## Current App Behavior

The root Pages site is a launcher with links to both app folders.

The HuTao Bet Assistant app has three tabs:

- `Calculator` for match inputs, market odds, AH, O/U, Kelly sizing, and recommendations.
- `History` for locally stored bet logs, pending/win/loss/skip filters, CLV entry, and clearing history.
- `Stats` for win rate, ROI, P/L, skipped count, CLV summary, and league breakdown.

Data persistence is browser-local via `localStorage` key `hutao_bets`.

## Known Issues And Cleanup Notes

- Some text appears to contain mojibake from older encoding conversion, such as intended arrows/dashes displaying as garbled character sequences.
- The project is currently a static app with no package manager, build step, automated tests, or CI.
- The roadmap calls for future automation, AI insights, odds format conversion, richer AH/O/U logic, and centralized logging.
- Responsible gambling language should remain present in prompts and recommendations. Never present the model as certainty.

## Baseline Principle

Treat the current static app and `Additional_Bet_skill` folder as the baseline. Future changes should preserve working standalone browser behavior unless the project explicitly moves to a framework.

For GitHub Pages, publish from the `Bet_assist_app` branch root so both folder links are available:

- `/main-app/`
- `/bet-assist-app/`
