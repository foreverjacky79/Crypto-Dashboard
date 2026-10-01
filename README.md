# Ticker — Crypto Dashboard

A browser-based, Traditional Chinese crypto watch terminal powered by OKX public
market data. It runs entirely on the client and is designed for GitHub Pages.

## Live site

After GitHub Pages is enabled for this repository, the dashboard is published at:

<https://foreverjacky79.github.io/Crypto-Dashboard/>

## Features

- Real-time OKX ticker and candlestick updates through public WebSockets.
- Watchlist, chart intervals, technical indicators, alerts, annotations, and
  drawing tools.
- Browser-local persistence for personal settings; no account, server, or API key.
- Responsive single-page interface that can be opened locally or deployed as a
  static site.

## Run locally

```bash
python3 -m http.server 4173
```

Open <http://localhost:4173/> in a browser. Internet access is required for live
OKX market data. The dashboard gracefully keeps its interface available if data
cannot be fetched.

## Deploy to GitHub Pages

The repository includes [the Pages workflow](.github/workflows/deploy-pages.yml).
In GitHub, open **Settings → Pages**, choose **GitHub Actions** as the source, and
push or merge to `main`. The workflow publishes the repository root, whose entry
point is `index.html`.

## AI-agent collaboration

Read [AGENTS.md](AGENTS.md) and [CONTRIBUTING.md](CONTRIBUTING.md). They document
the static-site constraints, validation expectations, and a safe handoff format
for multiple agents working on the dashboard.
