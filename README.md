# UnscrollMe

*Unwind, then begin.*

Small, quiet activities for an ADHD mind to come down after a scrolling session. One self-contained page: no build step, no accounts, no tracking, and no external requests (fonts are embedded, so it also works offline once loaded).

## What's inside

- **The reset** — unwind, then get one thing started. Check in (how loud is your head, 1–5), one minute of breathing, park what's looping, 5-4-3-2-1 grounding, then:
  - **Land**: pick one thing (your parked thoughts are offered as options) and write its first step, small enough to do in two minutes.
  - **Launch**: 30 seconds of light activation (stand, quick breaths, shake out hands, roll shoulders), then choose 5, 10 or 25 minutes.
  - **Focus**: a timer with your task and first step on screen, optional brown noise, +5 min, and a box to park stray thoughts without leaving.
  - **Finish**: shows what you started, how long you focused, the before/after number, and how many things you've started here. "Another round" gives a 1-minute breathing reset before the next timer.
- **One thing** — the Land → Launch → Focus path on its own, for when you're already calm enough.
- **Breathe** — a breathing circle with three patterns (long exhale 4·6, double-in sigh, box), 1/3/5 min or untimed, optional soft tones and vibration so you can close your eyes.
- **Park a thought** — type what's looping and let it drift across a stream, or save it to a "for later" list (kept in this browser only).
- **Follow the dot** (standalone) — one slow Lissajous path to track with a finger or your eyes; it glows while you stay with it.
- **Slow lines** — draw with a finger; fast strokes barely show, slow strokes glow. Everything fades on its own.
- **5 · 4 · 3 · 2 · 1** — tap-through sensory grounding.
- **Rest your eyes** — 90 seconds off the screen, dark overlay, a chime marks each step.
- **Brown noise** — toggle in the header, generated in the browser.

It follows the system light/dark setting and respects reduced-motion preferences.

## Publish on GitHub Pages

1. On github.com, create a new public repository, e.g. `unscrollme`.
2. Upload `index.html` and this `README.md` (Add file → Upload files → Commit).
3. Go to **Settings → Pages**. Under *Build and deployment*, set **Source: Deploy from a branch**, **Branch: `main`**, folder **`/ (root)`**, then Save.
4. After a minute the site is live at `https://<your-username>.github.io/unscrollme/`.

Or from a terminal:

```bash
git init && git add . && git commit -m "UnscrollMe"
git branch -M main
git remote add origin https://github.com/<your-username>/unscrollme.git
git push -u origin main
```

then enable Pages as in step 3.

## Note

This is a calm-down tool, not treatment.
