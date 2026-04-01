# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal academic/portfolio website for Tianpei Gu, hosted on GitHub Pages at https://gutianpei.github.io. Based on the [Clarity](https://shikun.io/projects/clarity) template by Shikun Liu (CC BY-SA 4.0).

## Architecture

This is a static single-page site with no build system or framework:

- **`index.html`** — The entire site in one file. Sections: title/hero, research publications, work experience, education, about, services, and contact. Each section uses `id` attributes for navigation (e.g., `#research-section`, `#work-section`).
- **`styles.css`** — All styling, using CSS custom properties for theming (color palette defined in `:root`). Uses custom fonts (Athletics, Tiempos Text) loaded from `assets/fonts/` and Google Fonts (Poppins, Charter, Fira Code).
- **`assets/`** — Static assets: `img/` (photos, logos), `fonts/` (self-hosted font files), `teaser/` (publication teaser images/videos).

## Development

No build step. Open `index.html` in a browser or use any local server:

```
python3 -m http.server 8000
```

CSS is cache-busted via query parameter (`styles.css?v=79`) — increment the version number when changing styles.

## Font Licensing

Athletics and Tiempos Text fonts are under personal/test licenses for non-commercial use only. They must not be redistributed. See README.md for details.
