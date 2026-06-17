# presentations

Single home for all WeAssist presentation decks, served via GitHub Pages.

**Live:** https://mark-weassist-io.github.io/presentations/

## Layout (rot-proof, future-proof)

```
presentations/
├── index.html            # dynamic table-of-contents — renders cards from the manifest
├── presentations.json    # MANIFEST — single source of truth (data, not code)
├── decks/
│   └── <slug>/index.html # one self-contained deck per folder
├── .nojekyll             # serve files verbatim (no Jekyll processing)
└── README.md
```

### Why it won't rot
- **Folder-per-deck** (`decks/<slug>/index.html`) → every deck has a clean URL (`/decks/<slug>/`) and **never 404s on direct land**.
- **Data-driven index** → the TOC reads `presentations.json`; nothing is hand-linked, so links can't go stale.
- **Decks are self-contained** single HTML files (fonts via CDN, no build step, no shared JS to break).

## Add a presentation
1. Create `decks/<slug>/index.html` (a self-contained deck).
2. Prepend an entry to `presentations.json` (newest first):
   ```json
   { "slug": "<slug>", "title": "...", "summary": "...", "date": "YYYY-MM-DD", "tags": ["..."] }
   ```
3. Commit & push. The index picks it up automatically — no code changes.
