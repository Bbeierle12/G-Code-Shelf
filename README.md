# G-code Shelf feed

The content feed for Brandon's G-code Shelf Android app.

- `feed.json` — manifest, newest first: title, date, file, size, SHA-256 per article.
- `index.html` — human-readable shelf list.
- `articles/` — full article HTML, exactly as published, newest first in the manifest.

The app fetches `feed.json` on open, downloads any new or changed articles, and caches them locally for offline reading. It does not need a new app version when an article is added — only this feed changes.
