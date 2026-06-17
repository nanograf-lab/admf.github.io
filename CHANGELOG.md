# CHANGELOG.md
# ADMF — Change Log

Chronological record of changes to the site, assets, and project.
For decisions and reasoning, see DECISIONS.md.

---

## 2026-06-17

- Created project documentation structure: README.md, PROJECT_CONTEXT.md, COPY_GUIDELINES.md, OUTREACH_LIBRARY.md, CHANGELOG.md, DECISIONS.md
- Established REFERENCES/ folder structure

---

## 2026-06-01

- `index-v2.html` created with approved hero copy and updated CTA
- `index-v2.html` marked as approved candidate; not yet deployed
- Font changed from Inter to Work Sans 400 + 600

---

## 2025–2026 (Site Build)

- Site migrated from Readymag to static HTML on GitHub Pages
- Repo created: github.com/nanograf-lab/admf.git
- CNAME configured: admf.work
- Desktop video: Video/ad_d.mp4
- Mobile video: Video/ad_m.mp4
- CSS custom properties implemented for light/dark theming
- Mobile values derived from 614px Figma canvas in vw units
- Mobile breakpoint: max-width 768px
- `overflow-x: clip` used (not `hidden`) to preserve sticky behaviour
- `.hero` set to `position: sticky; top: 0; z-index: 0`
- Credentials deck added to repo: admf.work_credentials.pdf

---

## Format for future entries

```
## YYYY-MM-DD

- What changed
- File affected
- Deployed: yes / no
```
