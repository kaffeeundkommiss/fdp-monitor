# fdp-monitor
Overview of FDP polling results (Bundestag + Landtagswahlen), sorted by election date (`index.html`),
plus a page with statistics on the party at federal level since 1998 (`partei.html`) and one on the topics of its election manifestos (`programme.html`); both read `partei.json` via `partei-seite.js` and `partei.css`.

## Tests

```
pip install -r requirements-dev.txt && pytest              # update.py
npm install && npm test                                    # monitor-utils.js, partei-utils.js (Vitest)
npm install && npx playwright install chromium && npm run test:e2e   # index.html, partei.html, programme.html (Playwright)
```
