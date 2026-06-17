# DECISIONS.md
# ADMF — Decision Log

Every important decision is documented here with date, change, and reason.
This file is the memory of the project.

---

## 2026-06-17

### CTA copy changed

**From:** "Read more"
**To:** "See how we work"

**Reason:** The linked PDF is a credentials deck, not a portfolio. "Read more" implies editorial content. "See how we work" accurately describes what the document contains and sets the right expectation.

**Status:** Approved. Implemented in `index-v2.html`. Not yet deployed to live site.

---

## 2026-06-17

### Hero copy — new candidate approved

**From (live):**
"A creative partner supporting businesses with clear design direction, visual craft, and the smart use of AI."

**To (approved candidate):**
"A senior multidisciplinary design partner.
Visual craft and product thinking, without the overhead of a traditional agency."

**Reason:** "Creative partner" is softer and more generic. It loses the seniority signal and the agency contrast — both doing real positioning work. The approved candidate is more specific, more confident, and more differentiated.

**Status:** Approved. Stored in `index-v2.html`. Not yet deployed. Deliberate — this is a positioning decision, not a technical task.

---

## 2026-06-17

### Site platform migrated

**From:** Readymade (Readymag)
**To:** Static HTML on GitHub Pages

**Reason:** Built with Claude Code. Full control over code, no platform dependency, direct deployment via git push.

**Repo:** github.com/nanograf-lab/admf.git
**Branch:** main
**Live:** admf.work

---

## 2026-06-17

### Font changed

**From:** Inter
**To:** Work Sans 400 + 600

**Reason:** Better match to visual direction. Inter removed entirely.

---

## 2026-06-17

### Project documentation structure established

**Decision:** Create a single source of truth inside `ADMF Site/` repo containing:
- `README.md`
- `PROJECT_CONTEXT.md`
- `COPY_GUIDELINES.md`
- `OUTREACH_LIBRARY.md`
- `CHANGELOG.md`
- `DECISIONS.md`
- `REFERENCES/`

**Reason:** ADMF is being worked on across Claude Chat, Claude Code, and Cowork. Without shared documentation, context is lost between sessions. These files ensure any Claude agent — or future collaborator — can orient themselves without reading chat history.
