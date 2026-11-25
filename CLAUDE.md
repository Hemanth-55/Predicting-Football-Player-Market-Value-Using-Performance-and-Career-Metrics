# Predicting Football Player Market Value: session context

Predicts player market value from performance and career metrics across top European leagues, then flags undervalued transfer targets.
Claude: read this file, then `notes/`, at the start of every session.

## The project
- Right now the repo is a README + assets only. The code and notebook aren't committed yet.
- Reported results (from README): Gradient Boosting R² 0.612, ~80% better than linear baselines, €1.7M lower valuation error per player, 64 undervalued targets.
- Method: log-transformed skewed features, SMOTE rebalancing, gradient boosting vs linear baselines.
- Open item: add the code/notebook so the results are reproducible. Ask Hemi where the original work lives before writing anything new.

## Rules
- **North star:** Hemi is becoming a consultant / advisor to the sports industry. Frame every output (README, demo, deck, résumé line) as decision → data → logic → recommendation → impact. See https://github.com/Hemanth-55/Tamil-/blob/main/notes/north-star.md
- Apple-level quality: minimal, professional, clear to a layman at a glance. Speak to tech people, no gimmicks.
- Never describe projects as done at BU.
- Never commit secrets, raw licensed data or large media.

## Session routine
- Start: `/session-start` · End: `/session-end` (log, commit, `git pull --rebase`, push)
- Several sessions can share this repo; the notes are the shared memory. Facts come only from the repo, the notes and Hemi. Ask, don't guess.

## Related
- Hub: https://github.com/Hemanth-55/Tamil- (index of all repos in `notes/repos.md`)
- Portfolio: https://github.com/Hemanth-55/Portfolio-Website (live: hemanthkumargopi.vercel.app)
