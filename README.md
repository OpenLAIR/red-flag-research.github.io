# Red-flag Research · Public site

- Project homepage: https://openlair.github.io/red-flag-research.github.io/
- Live page: https://openlair.github.io/red-flag-research.github.io/live/

## Layout

- `index.html`, `data/` — project homepage. The schedule, update cards and site text (product name, contact e-mail, repository URL) live in `data/schedule.json`, `data/updates.json` and `data/site.json`, not in the HTML.
- `live/` — live page (`index.html`, `data.js`, `sessions/`). It reads the public read-only API while a batch runs; otherwise it replays saved sessions from `data.js` and `sessions/` (exported events, Jev scores and short public excerpts; no local paths or credentials). Old root links with `?api=`, `?votes=` or `#pipeline` are forwarded to `live/`.
- `404.html` — not-found page with links to the live page and the homepage.

GitHub Pages publishes the reviewed static files from main. The pipeline runs on a separate host; the editor and provider credentials are not included.

## Benchmark

The benchmark is not hosted on this site. An anonymized release is published in the project's GitHub repository.
