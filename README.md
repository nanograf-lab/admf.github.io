# ADMF
## admf.work

Senior design partnership. Static site on GitHub Pages.

---

## Live Site

**URL:** https://admf.work
**Repo:** github.com/nanograf-lab/admf.git
**Branch:** main
**Platform:** GitHub Pages

---

## File Structure

```
ADMF Site/
├── index.html                  ← current live version
├── index-v2.html               ← approved copy candidate (not yet deployed)
├── admf.work_credentials.pdf   ← credentials deck (linked from site)
├── CNAME                       ← domain: admf.work
├── Video/
│   ├── ad_d.mp4                ← desktop video
│   └── ad_m.mp4                ← mobile video
├── REFERENCES/
│   ├── websites/
│   ├── copy/
│   ├── visual-direction/
│   └── competitors/
├── README.md                   ← this file
├── PROJECT_CONTEXT.md          ← what ADMF is, who it's for, full context
├── COPY_GUIDELINES.md          ← approved copy, tone rules, writing checklist
├── OUTREACH_LIBRARY.md         ← outreach principles and message templates
├── CHANGELOG.md                ← chronological record of changes
└── DECISIONS.md                ← log of important decisions and reasons
```

---

## Current State

- Live site serves `index.html` — contains older copy
- `index-v2.html` contains approved hero copy and CTA — awaiting deployment decision
- See DECISIONS.md for full context on the copy situation

---

## Deploy

```bash
git add .
git commit -m "your message"
git push origin main
```

GitHub Pages rebuilds automatically. Allow 1–2 minutes.

If push is rejected:
```bash
git pull --rebase origin main
git push origin main
```

---

## Tech Notes

- `overflow-x: clip` on `html, body` — not `hidden` (breaks `position: sticky`)
- `.hero` is `position: sticky; top: 0; z-index: 0` — video slides over it via `z-index: 1`
- CSS custom properties: `--bg`, `--text`, `--knob`, `--track`, `--border` — theme via `data-theme` on `<html>`
- Font: Work Sans 400 + 600 (Google Fonts) — Inter removed
- Mobile values in `vw` units from 614px Figma canvas: `px / 614 × 100`
- Mobile breakpoint: `max-width: 768px`
- `.hero h1` requires explicit `font-weight: 400` — browser UA overrides with bold
- Desktop line break: `<br class="desktop-break">` with `display: block` / `display: none` in media query
- Dark mode: button uses `color: var(--bg); background: var(--text)` — never hardcode colours

---

## Figma

**File:** https://www.figma.com/design/mdcR1scmUF8cADITbouHns/Claude-Code-Lab
**ADMF frame:** node 44:2 (page "am.com", x=17400)
**Desktop frames:** node 36-2

---

## Documentation

| File | Purpose |
|---|---|
| PROJECT_CONTEXT.md | Full business context — read this first |
| COPY_GUIDELINES.md | Approved copy, tone, writing rules |
| OUTREACH_LIBRARY.md | Outreach principles and templates |
| CHANGELOG.md | What changed and when |
| DECISIONS.md | Why things are the way they are |

---

## PDF Note

Two copies of the credentials deck exist:

- `site/admf.work_credentials.pdf` — deployed website asset (this file)
- `docs/admf.work_credentials.pdf` — working/source copy

When updating the credentials deck, update both.

---

## Contact

hello.admf@gmail.com
