# Base44 Dev Environment

This is a single-file static personal portfolio (`index.html`) — no build step, no backend, no external services or secrets.

## Running
```
docker compose -f docker-compose.base44.yml up -d
```
Serves `index.html` on port 3000 via `npx serve` (binds 0.0.0.0, accepts any host).

## Verifying
- `curl -sf -H "Host: external.example.com" http://localhost:3000/` returns the HTML.
- Preview should show the portfolio landing page.

## Editing
All changes live in `index.html` (HTML + CSS + JS in one file). The static server picks up edits on refresh — no reload step needed.
