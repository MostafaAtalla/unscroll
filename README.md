# Unscroll

Small, quiet activities for an ADHD mind to come down after a scrolling session. One self-contained page: no build step, no accounts, no tracking, no external assets except two Google Fonts.

## What's inside

- **5-minute reset** — a guided sequence: check in (how loud is your head, 1–5), one minute of breathing, park what's looping, 90 seconds following a slow dot, 5-4-3-2-1 grounding, check out.
- **Breathe** — a breathing circle with three patterns (long exhale 4·6, double-in sigh, box), 1/3/5 min or untimed, optional soft tones and vibration so you can close your eyes.
- **Park a thought** — type what's looping and let it drift across a stream, or save it to a "for later" list (kept in this browser only).
- **Follow the dot** — one slow Lissajous path to track with a finger or your eyes; it glows while you stay with it.
- **Slow lines** — draw with a finger; fast strokes barely show, slow strokes glow. Everything fades on its own.
- **5 · 4 · 3 · 2 · 1** — tap-through sensory grounding.
- **Rest your eyes** — 90 seconds off the screen, dark overlay, a chime marks each step.
- **Brown noise** — toggle in the header, generated in the browser.

It follows the system light/dark setting and respects reduced-motion preferences.

## Publish on GitHub Pages

1. On github.com, create a new public repository, e.g. `unscroll`.
2. Upload `index.html` and this `README.md` (Add file → Upload files → Commit).
3. Go to **Settings → Pages**. Under *Build and deployment*, set **Source: Deploy from a branch**, **Branch: `main`**, folder **`/ (root)`**, then Save.
4. After a minute the site is live at `https://<your-username>.github.io/unscroll/`.

Or from a terminal:

```bash
git init && git add . && git commit -m "Unscroll"
git branch -M main
git remote add origin https://github.com/<your-username>/unscroll.git
git push -u origin main
```

then enable Pages as in step 3.

## Note

This is a calm-down tool, not treatment.
