# AK Beads Studio

The public website for AK Beads Studio — premium beads, handmade jewelry and keychains. It is a single self-contained HTML page (styles, scripts and images are all embedded) with a product catalog, category filters, a cart, FAQ, and an owner panel for editing products, categories and settings.

## Technologies
- Plain HTML, CSS and JavaScript (no build step)
- Hosted on Netlify, published from the `public/` folder

## Run locally
Open `public/index.html` in a browser, or run `netlify dev --port 8889` from the project root.

## Roadmap
- Owner edits (products, categories, settings) and the cart are currently saved in each visitor's browser only. Moving them to Netlify Database would make owner changes visible to every visitor.
- The owner login is checked in the browser; moving it to Netlify Identity would make it secure.
