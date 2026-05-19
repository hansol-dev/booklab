# Booklab Renewal Agent Notes

This repository contains the Booklab renewal prototype currently deployed through GitHub/Vercel.
Use this file as the handoff note when a new terminal or new agent session starts.

## Workspace

- Root: `C:\hansol\booklab`
- Main prototype: `prototype/booklab-renewal/`
- Main files:
  - `prototype/booklab-renewal/index.html`
  - `prototype/booklab-renewal/styles.css`
  - `index.html` redirects the Vercel root to `./prototype/booklab-renewal/`
- Live preview checked by the user: `https://booklab-coral.vercel.app/`

## Current Design Direction

- This is not a 1:1 clone of the old Booklab site.
- The design keeps Booklab's existing content, but renews it with a cleaner, modern structure inspired by Good Ground-style content density and homepage flow.
- Important content blocks currently in the prototype:
  - Header with search, contract consultation phone, member links, and GNB.
  - Mobile hamburger menu with accordion 1-depth/2-depth navigation.
  - Main hero slider with fixed-size slides and generated visual images.
  - Service section with three service cards and button groups.
  - Hall of Fame, Bookstore/New Books, Self Interview sections with script-style decorative labels.
  - NEWS, Story, Payment/Consultation cards.
  - Author quick menu.
  - Footer based on Booklab company/footer content.

## Recent State

Recent pushed commits:

- `8ccac8f Fix mobile footer layout`
- `9efa150 Adjust mobile payment card layout`
- `a9589b2 Fix story more link alignment`
- `c60b7d6 Improve mobile navigation and section headers`
- `5c2d5f1 Add mobile hamburger menu`

Recent fixes already applied:

- Mobile footer no longer overflows; footer links are two-column buttons on mobile.
- Mobile payment/consultation card places credit-card payment on the left and phone numbers on the right.
- `Booklab Story` lower card `more` link is right-aligned.
- Mobile menu uses hamburger button and accordion submenus.
- Mobile title/script/button alignment was adjusted.

## Git And Deployment

- Remote: `https://hansol-dev@github.com/hansol-dev/booklab.git`
- Branch: `main`
- Git commands usually need:
  - `git -c safe.directory=C:/hansol/booklab status --short`
  - `git -c safe.directory=C:/hansol/booklab add <files>`
  - `git -c safe.directory=C:/hansol/booklab commit -m "<message>"`
  - `git -c safe.directory=C:/hansol/booklab push`
- Push is already approved in prior sessions with this prefix:
  - `git -c safe.directory=C:/hansol/booklab push`
- Vercel deploys from GitHub after push. Allow a short delay before checking the live URL.

## Editing Rules For This Project

- Use `apply_patch` for manual file edits.
- Use `rg` for searching.
- Do not revert unrelated changes.
- There is an untracked `mobile.png` screenshot in the root. Do not commit it unless the user explicitly asks.
- Be careful with Korean text display in PowerShell: `Get-Content` may show mojibake even when the file is fine. Prefer `rg` or browser rendering for text checks.
- After CSS edits, verify braces:
  - `$css = Get-Content -Raw -Path prototype/booklab-renewal/styles.css; $open = ([regex]::Matches($css, '\{')).Count; $close = ([regex]::Matches($css, '\}')).Count; "open=$open close=$close"`
- If JS is touched, run a syntax check or inspect carefully before committing.

## Visual Assets

Generated/current hero and service assets are in:

- `prototype/booklab-renewal/assets/service/main-hero-publishing-journey.png`
- `prototype/booklab-renewal/assets/service/main-hero-distribution.png`
- `prototype/booklab-renewal/assets/service/main-hero-printing.png`
- `prototype/booklab-renewal/assets/service/service-tools-warm.png`
- `prototype/booklab-renewal/assets/service/service-printing-warm.png`

Local font:

- `prototype/booklab-renewal/assets/fonts/PretendardVariable.woff2`

## User Preferences

- User wants iterative visual refinement, especially mobile polish.
- Avoid making the site look like an exact copy of the old Booklab homepage.
- Keep Booklab's real content, menu labels, phone numbers, services, books, news/story/interview content.
- User dislikes overly red-heavy UI and asks for cleaner, less dated buttons.
- Use `word-break: keep-all` broadly where Korean text wraps awkwardly.
- When asked to deploy visible changes, commit only relevant files and push to `main`.
