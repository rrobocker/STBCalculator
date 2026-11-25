# Brainrot Toolkit V2.0

Upload both HTML files and the entire data folder to the existing GitHub Pages repository root. Keep relative paths intact. No build step is required.

## Updating data
- brainrots.json: shared list of name, rarity, baseIncome (raw dollars per second). Keep names unique.
- mutations.json and traits.json: income multipliers.
- level-multipliers.json: existing estimated level curve (index 0 unused), measured anchor levels.
- eternal-machine.json: outcome names, normal/premium tier tables (columns follow outcomeNames), mutation odds, provisional observed threshold and odds. Special recipe logic remains in eternal-machine.html.

Use valid JSON (no trailing commas). Test on GitHub Pages or run `python -m http.server 8000` in this directory and visit http://localhost:8000. Opening HTML directly from disk may block JSON fetches.

Existing datamining attribution to Adamo and player-observed caveats are retained in the HTML. No new game data was inferred.
