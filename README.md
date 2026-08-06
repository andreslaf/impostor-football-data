# impostor-football-data

Hosted player dataset for the Impostor Football app, served via GitHub Pages.

- `players.json` — the full player dataset (`{version, players[]}`).
- `players-meta.json` — `{version}` only; the app polls this to decide whether to fetch a newer `players.json`.

To publish an update: replace `players.json`, bump its `version`, set the same number in `players-meta.json`, and `git push`. Apps pick it up on their next-but-one launch — no app-store submission required.
