# Bevin John — portfolio

An editorial, project-first portfolio for Bevin John. Built as a static site with HTML, CSS, and JavaScript; **no build step or npm install**.

## What's included

- `index.html` — entry point, SEO metadata, semantic landmarks, contact/GitHub dialogs
- `assets/styles.css` — responsive design system
- `assets/app.js` — project filtering, search, navigation, case studies, popups
- `assets/projects.js` — project data and detailed case-study content
- `assets/favicon.svg` — brand icon
- `.nojekyll` — makes GitHub Pages serve files without Jekyll processing
- `DEPLOY.md` — step-by-step guide to GitHub Pages and your own domain

## Open locally

Double-click `index.html` after extracting the ZIP. The site works without a backend. Google Fonts need an internet connection; system fallback fonts are available offline.

## Personalize

- Edit project details in `assets/projects.js`.
- Edit visible profile copy, career information, and button labels in `assets/app.js`.
- Edit contact details in `index.html` (search for `bevinjohn22@gmail.com` or `847-990-0938`).
- Edit colors and spacing in `assets/styles.css`.

## Content and attribution

The case studies retain the previous portfolio's seven selected projects and descriptions. Public repositories are linked when verified. Private/internal and developer-described implementations are labeled as conceptual overviews. Forks and class exercises are explicitly labeled as coursework, not original independent software.

**Before publishing:** review the Grey-box Codex description for any employer-confidential information, and verify every implementation and achievement against current work. If you later make Veil public, add the correct GitHub repository URL to its `repo` field in `assets/projects.js`.

## Features tested

Desktop and mobile layout, all seven cards, search, filters, hash-routing case studies, About page, contact popup, GitHub-profile chooser, and absence of horizontal overflow. The project has no server-side code or telemetry.
