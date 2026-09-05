# CA Intermediate Study Planner

A personal study planner PWA for CA Intermediate exam prep — all 6 papers (Advanced Accounting, Corporate & Other Laws, Taxation, Cost & Management Accounting, Auditing & Ethics, Financial & Strategic Management) with chapter-level tracking, daily planner, Pomodoro timer, analytics, revision scheduler, calendar, and goals.

Works fully offline once installed, and all your data stays on your device (saved in browser `localStorage` — nothing is sent to a server).

## 1. Push this to GitHub

From inside this folder:

```bash
git init
git add .
git commit -m "Initial commit: CA Intermediate study planner PWA"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo-name>.git
git push -u origin main
```

(Create the empty repo on GitHub first at github.com/new — don't add a README/license there, since this folder already has one.)

## 2. Turn on GitHub Pages

1. On GitHub, go to your repo → **Settings** → **Pages**.
2. Under "Build and deployment", set **Source** to `Deploy from a branch`.
3. Set **Branch** to `main` and folder to `/ (root)`. Save.
4. Wait ~1 minute, then your app will be live at:
   `https://<your-username>.github.io/<your-repo-name>/`

## 3. Install it as an app on your phone

- **Android (Chrome):** open the link above → tap the ⋮ menu → **Add to Home screen**.
- **iPhone (Safari):** open the link above → tap the Share icon → **Add to Home Screen**.

It'll then open full-screen with its own icon, and keep working without internet.

## Updating later

Whenever you want to change chapter names, colors, or add a feature, edit `index.html` and:

```bash
git add .
git commit -m "Update planner"
git push
```

GitHub Pages redeploys automatically within a minute.

## Files

- `index.html` — the entire app (UI + logic)
- `manifest.json` — PWA metadata (name, icons, colors)
- `sw.js` — service worker, caches the app for offline use
- `icons/` — home-screen icons
- `.nojekyll` — tells GitHub Pages to serve files as-is

## Data & backup

Your data lives in your browser's local storage on whichever device you use it on — it does **not** sync between devices automatically. Use **More → Backup → Export data** regularly, especially before clearing browser data or switching phones, and **Import data** to restore it.
