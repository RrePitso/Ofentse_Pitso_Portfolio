# Ofentse Pitso — Portfolio

My personal portfolio site — built to show real, deployed work rather than a list of claims. Live at:

**https://rrepitso.github.io/Ofentse_Pitso_Portfolio/**

## About

A single-page site covering who I am, what I've built, and how to reach me — aimed at employers looking at me for AI / software engineering roles. Sections: Home, About, Skills, Projects, Experience, Education & Certifications, Contact.

## Tech stack

Deliberately simple — no framework, no build step, nothing to install:

- **HTML, CSS, vanilla JavaScript** — one file, `index.html`
- **[Google Fonts](https://fonts.google.com/)** — Newsreader (headings) and IBM Plex Sans / IBM Plex Mono (body and labels), loaded via CDN
- **[GitHub Pages](https://pages.github.com/)** — hosting, deployed straight from the `main` branch

No React, no npm, no package.json. The whole site is readable top to bottom in one file.

## Project structure

```
Ofentse_Pitso_Portfolio/
├── index.html              # the entire site — markup, styles, and script
├── Profile.jpg              # profile photo used in the sidebar
├── CV-Ofentse-Pitso.pdf     # downloadable CV, linked from the hero section
└── README.md
```

## Running locally

No build tools needed. Either:

- Open `index.html` directly in a browser, or
- Serve it locally so relative paths and fonts behave exactly as they do in production:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deployment

Hosted on GitHub Pages, configured under **Settings → Pages**:

- **Source:** Deploy from a branch
- **Branch:** `main` / `(root)`

Any commit to `main` that touches `index.html` rebuilds the live site automatically, usually within a minute or two.

## Updating content

Everything lives in `index.html`, organized into commented sections (`<!-- HERO -->`, `<!-- PROJECTS -->`, `<!-- EXPERIENCE -->`, etc.) so a section can be found and edited without touching anything else. Colors, fonts, and spacing are defined once as CSS variables near the top of the file (`:root { ... }`) — changing a value there updates it everywhere it's used.

To swap the CV, replace `CV-Ofentse-Pitso.pdf` with a new file of the same name (or update the `href` on the "Download CV" button in the Home section).

## Contact

- GitHub: [github.com/RrePitso](https://github.com/RrePitso)
- LinkedIn: [linkedin.com/in/ofentse-pitso](https://linkedin.com/in/ofentse-pitso)
