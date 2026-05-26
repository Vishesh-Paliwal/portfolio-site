# Portfolio &mdash; Vishesh Paliwal

A minimal, content-first personal site. No build step, no framework &mdash; just `index.html`, `styles.css`, and a tiny `script.js`.

## Run locally
```bash
# any static server works; pick one:
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploy
- **GitHub Pages**: push to a repo, settings &rarr; Pages &rarr; deploy from `main` branch root.
- **Vercel / Netlify / Cloudflare Pages**: drag the folder into the dashboard, or `vercel --prod`.
- **Custom domain**: any of the above + a CNAME.

## Placeholders to fill
Search `index.html` for `{{ ... }}` and replace:
- `{{LINKEDIN_URL}}` &mdash; your LinkedIn profile URL
- `{{TWITTER_URL}}` &mdash; your X/Twitter URL (or remove the link + separator)
- `{{RESUME_URL}}` &mdash; link to a hosted PDF (e.g. /resume.pdf)
- `{{NOW_BLURB}}` &mdash; what you're up to right now (1&ndash;2 sentences, paco.me-style)
- `{{JURY_URL}}` &mdash; The Jury repo or demo URL

## Design notes
- Single-column, ~680px max width
- Serif display heading (system serifs), sans-serif body, mono for meta/labels
- Light theme uses a warm off-white; dark theme uses near-black
- One accent color (warm rust / coral), used sparingly on hover, selection, and highlights
- Theme respects `prefers-color-scheme`, persisted in `localStorage`
- Zero external dependencies, zero tracking, zero JS frameworks
