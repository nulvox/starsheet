# starsheet

[![Use this template](https://img.shields.io/badge/Use%20this%20template-2ea44f?logo=github)](https://github.com/nulvox/starsheet/generate)

A GitHub template for single-source resumes. Write your resume in Markdown,
get a polished web page plus downloadable PDF, DOCX, and RTF exports. The
HTML page has a floating export bar; the other formats include a "View
online" link back to the canonical URL.

Demo content lives in `src/content/resume.md` and renders as a fictional
resume so you can see what the output looks like before customizing.

## Make this your own resume

1. On [github.com/nulvox/starsheet](https://github.com/nulvox/starsheet),
   click **"Use this template" → Create a new repository**. (Or use the
   [direct link](https://github.com/nulvox/starsheet/generate).) Pick your
   own repo name; the new repo starts with no history.
2. Clone your new repo locally.
3. Replace the demo content. The places you need to touch:
   - `src/content/resume.md` — your name, contact info, and resume body.
     Delete the demo callout at the top.
   - `package.json` — change `"name"` and `"version"` if you want.
   - `README.md` — replace this file with whatever describes your project.
   - **If you're not deploying via GitHub Pages**, also update
     `astro.config.mjs` (`site:`) and `Makefile` (`SITE_URL ?=`) to point
     at your hosting URL. The Pages workflow fills these in automatically
     from `actions/configure-pages` outputs, so you can leave them
     untouched if you're using the included workflow.

   The PDF page footer and any leftover `https://ada.example.com` strings
   in the source are automatically rewritten to `$SITE_URL` at build
   time, so you don't need to edit `src/styles/print.css` by hand.
4. (Optional) Customize the DOCX look: see `templates/README.md`.
5. Build locally: `make` produces `dist/index.html` plus
   `resume.{pdf,docx,rtf}`.
6. Deploy. Two options:
   - **GitHub Pages** (auto): in your repo, go to **Settings → Pages** and
     set **Source: GitHub Actions**. Push to `main` and the included
     workflow (`.github/workflows/deploy.yml`) will build and publish.
     The workflow feeds the Pages URL into Astro's `site`/`base` and into
     `SITE_URL`, so it works on any forked repo without further edits.
   - **Anywhere else**: build with `make SITE_URL=https://your.example.com`
     and upload `dist/` to Netlify, Cloudflare Pages, S3, etc.

## Stack

- **Astro** — markdown processing, layouts, dev server, static output
- **Pandoc** — DOCX and RTF generation from the same markdown source
- **WeasyPrint** — PDF generation from the rendered HTML (CSS Paged Media)
- **Vanilla JS / CSS** — floating export bar, print styles

No client-side document generation. Exports are built once at build time
and served as static files, so the floating buttons are just `<a download>`
tags.

## Layout

```
.
├── src/
│   ├── content/
│   │   └── resume.md          # YOUR RESUME — edit this
│   ├── layouts/
│   │   └── Resume.astro       # HTML shell, injects export bar
│   ├── components/
│   │   └── ExportBar.astro    # floating PDF/DOCX/RTF buttons
│   ├── styles/
│   │   ├── resume.css         # screen styles
│   │   └── print.css          # @media print + WeasyPrint @page rules
│   └── pages/
│       └── index.astro        # entry — renders resume.md via the layout
├── templates/
│   ├── reference.docx         # Pandoc style reference (generate once)
│   └── footer.md              # auto-generated: "View online at ..."
├── scripts/
│   └── build-exports.sh       # runs Pandoc + WeasyPrint, drops into dist/
├── public/                    # static assets copied as-is (favicon, etc.)
├── astro.config.mjs
├── package.json
└── Makefile                   # one-shot: `make` builds everything
```

## Build

### 1. Install Node via nvm

[nvm](https://github.com/nvm-sh/nvm) is a per-user Node version manager —
no `sudo`, no fights with the system package set, easy to upgrade. Follow
the upstream install instructions at
<https://github.com/nvm-sh/nvm#installing-and-updating> (one curl command),
then:

```sh
nvm install 24       # matches the Node version pinned in CI
nvm use 24
npm install          # astro and the rest of the JS deps go here
```

### 2. Install pandoc and weasyprint

These two aren't on npm. On Ubuntu/Debian:

```sh
sudo apt-get update
sudo apt-get install -y pandoc weasyprint
```

Other platforms: `brew install pandoc weasyprint` (macOS),
`pacman -S pandoc python-weasyprint` (Arch). Any reasonably recent
version of either tool is fine.

### 3. Build

```sh
make                 # → dist/index.html + dist/resume.{pdf,docx,rtf}
make dev             # astro dev server on :4321
make clean
```

## How the back-link works

`scripts/build-exports.sh` regenerates `templates/footer.md` from the
`SITE_URL` make variable on every build. The footer is appended by Pandoc
when generating DOCX/RTF. The HTML build ignores it (the canonical URL is
already where you're reading it). Edit `SITE_URL` in the `Makefile` (or
pass it on the command line) to change it everywhere at once.

The PDF page footer lives in `src/styles/print.css` as literal CSS
content (so WeasyPrint can render it through `@page`). The build script
sed-substitutes the placeholder URL in the built HTML right before
WeasyPrint reads it, so the PDF footer ends up matching `SITE_URL`
without any manual edits to `print.css`.

## Customizing

- **Content**: edit `src/content/resume.md`. Frontmatter holds name,
  contact info, and theme toggles.
- **Style**: `src/styles/resume.css` for screen, `src/styles/print.css`
  for paged output. Both are consumed by WeasyPrint via Astro's built
  HTML, so the PDF matches the webpage closely.
- **DOCX look**: regenerate the reference doc with
  `pandoc -o templates/reference.docx --print-default-data-file reference.docx`,
  open it in LibreOffice, tweak styles, save. Pandoc will use it on next
  build.

## Forking this template itself

If you want to publish your own variant of starsheet (different defaults,
different stack, etc.), fork normally, then in **Settings → General**
check **"Template repository"** so others can "Use this template" from
your fork.
