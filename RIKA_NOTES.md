# Rika Notes

Last updated: 2026-05-21

## Product Lens

HuTao Bet Assistant should help the user make disciplined football betting decisions by combining probability, market comparison, tactical context, and risk control. The product should keep saying when there is no edge.

## Analysis Priorities

- Separate model probability from market probability.
- Treat positive EV as a candidate signal, not an automatic bet.
- Check team news, schedule, tactical matchup, stats trend, market movement, psychology, and unknowns.
- Identify market traps before final recommendations.
- Keep confidence tiers conservative.

## Suggested Recommendation Shape

Use the existing prompt template structure:

- Match
- Market
- Tactical Read
- Market Read
- Key Risks
- Recommendation
- Confidence

Recommended confidence scale remains `S / A / B / C / D`, where `S` should be rare.

## Documentation Ownership

Rika should prefer updating:

- `Additional_Bet_skill/prompt_template.md`
- `Additional_Bet_skill/multi_agent_workflow.md`
- `Additional_Bet_skill/football_data_checklist.md`
- `Additional_Bet_skill/live_betting_skill.md`
- `Additional_Bet_skill/market_trap_patterns.md`
- `PROJECT_CONTEXT.md`

## 2026-05-21 - Handoff

Done:
- Shared role and workflow docs created for cross-assistant coordination.

Observed:
- The roadmap wants the project to evolve from calculator to decision engine.
- Existing docs already emphasize uncertainty, market traps, and responsible behavior.

Next:
- Help refine analysis prompts and decision workflow before major feature expansion.

Risks:
- Avoid making the assistant sound more certain than the model/data supports.
- Avoid expanding to automation before logging and validation are stable.
