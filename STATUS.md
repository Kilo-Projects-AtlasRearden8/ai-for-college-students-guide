# STATUS — AI for College Students (Asdale Dynamics, LLC)

## What was built

A beginner manual for using free AI in college, delivered as both Markdown
(`docs/`) and a static HTML site (`site/`), plus a printable study planner.

### Contents
- `docs/index.md` — getting started + how to use the manual
- `docs/essay-brainstorming.md` — brainstorm essay angles and outlines
- `docs/study-guides.md` — turn notes into summaries, flashcards, quizzes
- `docs/citation-help.md` — MLA/APA/Chicago citation help with verification warning
- `docs/schedule-planning.md` — weekly schedule planning with AI
- `docs/email-drafts.md` — polite email drafts for professors/advisers/offices
- `docs/privacy.md` — privacy rules (never paste grades or ID numbers)
- `docs/study-planner.md` — printable study planner
- `site/` — static HTML mirror of all docs pages, one shared CSS file
- `site/planner.html` — printable one-page weekly study planner (A4)
- `LICENSE` — MIT, copyright line exactly "Copyright (c) 2026 Asdale Dynamics, LLC"
- `README.md` — project overview, credits Asdale Dynamics, LLC

No `.github/workflows` files. No build step required.

## How to run

It's a static site — nothing to install, no server, no internet needed once you have the files.

1. Open `site/index.html` in any web browser.
2. Browse chapters via the navigation bar.
3. Print `site/study-planner.html` (Ctrl+P / Cmd+P) for the one-page study planner.
   - Turn on "Background graphics" if you want colors; prints fine in B&W too.
4. Or read the Markdown files in `docs/` directly.

## Verification results

- HTML tag balance: all 8 site pages pass (no unclosed/unexpected tags)
- Internal links: no broken links across all site pages
- Secrets/scan: no API keys, passwords, or personal data found (all "student ID" / "password" mentions are privacy warnings telling users NOT to paste them)
- LICENSE copyright line: exactly "Copyright (c) 2026 Asdale Dynamics, LLC" (line 3)
- README: credits Asdale Dynamics, LLC and Dylan Asdale
- Git: initialized, committed on `master` as Dylan Asdale (no co-author trailers, not pushed)

## Known gaps

- No automated test suite (static HTML/Markdown; verification done manually via scripts)
- HTML not validated against a formal DTD/schema (tag balance + link checks performed instead)
- Print layout tested by CSS `@media print` rules only, not by an actual printer/PDF render
- The manual covers the five requested college topics (essays, study guides, citations, schedule, email) plus privacy and planner; broader LLC topics (agents/MCP, local AI, KDP, bookkeeping, healthcare aids, FFXIV, chess) are out of scope for this project
