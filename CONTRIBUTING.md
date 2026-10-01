# Contributing to Ticker

Thanks for improving this lightweight crypto dashboard. The project is a static,
client-only GitHub Pages site, so anyone (including AI coding agents) can work on
it without local services or credentials.

## Fast start

```bash
python3 -m http.server 4173
```

Then open `http://localhost:4173/`. Use a browser with network access to verify
live OKX market data. Personal watchlists, alerts, drawings, and annotations are
stored only in that browser's `localStorage`.

## Contribution checklist

1. Read [`AGENTS.md`](AGENTS.md) before changing files.
2. Keep changes focused and explain user-visible behavior in the pull request.
3. Do not commit credentials or add server-side dependencies.
4. Run the available static checks and a local smoke test.
5. Keep the GitHub Pages workflow intact; pushes to `main` deploy `index.html`.

## Collaboration notes for AI agents

Use one task per agent where possible (for example: chart rendering, accessibility,
or documentation). Avoid concurrent edits to the same blocks in `index.html`.
Include the files changed, commands run, and any limitations in your handoff so a
maintainer or another agent can safely continue the work.
