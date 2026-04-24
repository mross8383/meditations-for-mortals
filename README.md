# Meditations for Mortals — A 28-Day Companion

A self-guided, four-week interactive companion inspired by Oliver Burkeman's *Meditations for Mortals*. Built as a single-page web app: tap through weeks and days, work through reflections and small actions, and journal as you go.

**Live site:** [mross8383.github.io/meditations-for-mortals](https://mross8383.github.io/meditations-for-mortals/)

---

## What it is

Twenty-eight days of short, actionable reflections on living within finite time, organised across four themed weeks:

1. **Being Finite** — Confronting the truth of limited time
2. **Taking Action** — Moving forward without certainty
3. **Letting Go** — Releasing the need to control everything
4. **Showing Up** — Being present in the life you actually have

Each day contains a key idea, a short summary, a reflection question, a practical action, a completion checkbox, and a journal box for your own notes.

---

## What it isn't

This is **not** a reproduction of Oliver Burkeman's book. It's a structured companion written in the spirit of his thinking. The chapter titles, summaries and prompts here are interpretations, not extracts. If you find this useful, buy the book — it's worth your time.

---

## Features

- 28 days of structured reflections across 4 weeks
- Collapsible weeks and days for easy navigation
- Per-day journal with autosave
- Progress tracking (per week + overall)
- Fully offline-capable after first load
- Mobile-first design (iPhone, iPad, desktop)
- All data stored locally in your browser — no accounts, no tracking, no backend

---

## Privacy

All progress and journal entries are stored in your browser's `localStorage`. Nothing leaves your device. There is no analytics, no tracking, no server.

This also means:

- Data is **per-device, per-browser**. Entries on your iPhone won't appear on your iPad.
- Clearing your browser data will erase your progress.
- If you want a backup, copy your journal entries somewhere safe.

---

## Running locally

It's a single HTML file with no build step. Either:

**Option A — open directly:**
```
open index.html
```

**Option B — serve with Python (recommended for proper localStorage behaviour):**
```
python3 -m http.server 8000
```
Then visit [http://localhost:8000](http://localhost:8000).

---

## Deploying to GitHub Pages

1. Create a new public repo on GitHub (e.g., `meditations-for-mortals`).
2. Push the contents of this folder to the `main` branch.
3. Go to **Settings → Pages**.
4. Under **Source**, select **Deploy from a branch**.
5. Select **Branch: main**, **Folder: / (root)**, and click **Save**.
6. Wait 1–2 minutes. The site will be live at `https://<your-username>.github.io/<repo-name>/`.

The included `.nojekyll` file ensures GitHub doesn't try to process the site with Jekyll (not needed for a plain HTML file).

---

## File structure

```
.
├── index.html          # The app itself (single self-contained file)
├── README.md           # This file
├── LICENSE             # MIT licence
├── .nojekyll           # Tells GitHub Pages to skip Jekyll processing
├── .gitignore          # Standard ignores
└── 404.html            # Friendly 404 page
```

---

## Tech notes

- Single HTML file, no build step, no dependencies beyond Google Fonts (Fraunces, Inter, JetBrains Mono).
- Vanilla JavaScript, no frameworks.
- localStorage for persistence (two keys: `meditations-mortals-progress-v1`, `meditations-mortals-journals-v1`).
- Earthy green/brown palette, editorial typography, optimised for touch.

---

## Credits

Written and built as a personal companion. Inspired by — but not affiliated with or endorsed by — Oliver Burkeman or his publisher.

## Licence

MIT — see [LICENSE](LICENSE).
