# Letter Garden — Arabic & English Learning

A free, responsive learning website that runs entirely in the browser. No server, database, API key, or build step needed.

## Features

- All 28 basic Arabic alphabet letters with English transliteration and sound hints
- All 26 English alphabet letters
- Numbers **0–19** with Arabic-Indic digits, Arabic names and English names
- Click-to-hear pronunciation using the browser's built-in Web Speech API
- Flashcards, 10-question multiple-choice quizzes, search, saved learning progress
- Works on mobile and desktop, and can be hosted free on GitHub Pages

## Publish on GitHub Pages

1. Create a **public GitHub repository**, e.g. `letter-garden`.
2. Upload `index.html`, `style.css` and `app.js` to the **root** of your repo (or use Git).
3. Go to **Settings → Pages → Build and deployment**.
4. Set **Source** to **Deploy from a branch**; choose branch `main`, folder `/ (root)`, and click **Save**.
5. GitHub will show your site address, typically `https://YOUR-USERNAME.github.io/letter-garden/`.

If using the command line:

```bash
git init
git add .
git commit -m "Launch Letter Garden"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/letter-garden.git
git push -u origin main
```

## Test locally

Open `index.html` in a modern browser; or start a local server with `python3 -m http.server 8000` and visit `http://localhost:8000`.

## Notes

- Arabic pronunciation depends on the installed browser/device Arabic speech voices. On some devices Arabic playback may be unavailable or sound different; install an Arabic voice or use another browser.
- Arabic letter names and isolated letter sounds are not identical; the alphabet card audio uses letter characters and can vary by voice engine. English pronunciation hints are simplified learning aids, not a full phonetic description.
- Progress is stored **only on the current device/browser** in localStorage.
- Fonts load from Google Fonts when online; system fonts are used as fallback.
- Educational coverage is Modern Standard Arabic alphabet and numbers 0–19. This is a starter learning app, not a complete Arabic course.

## Files

- `index.html`: accessible page structure
- `style.css`: responsive design
- `app.js`: lesson data and interactions
