# AGENTS.md

## Architecture
- `public/index.html` is the entire site: one self-contained HTML file with inline CSS, inline JS and base64-embedded images (~2.5 MB). It was supplied by the owner — edit it in place rather than restructuring.
- `netlify.toml` publishes `public/` with no build command.

## Notes
- State (products, categories, category icons, settings, cart) lives in `localStorage` keys prefixed `ak` (`akProducts`, `akCats`, `akCatIcons`, `akSettings`, `akCart`). Owner session uses `sessionStorage.akOwner`.
- The owner login is a client-side check in `ownerLogin()`; credentials are visible in page source. Treat as a convenience gate, not security. Migrating to Netlify Identity + Netlify Database is the natural next step (see README roadmap).
