# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
npm run dev      # start Vite dev server at http://localhost:5173
npm run build    # production build
npm run preview  # preview production build
```

No linter, test runner, or type checker is configured.

## Architecture

Single-page Vite + Vanilla JS project. No framework, no bundler config beyond Vite defaults.

- `index.html` — entry point; contains a single `#card` div where all name card markup lives
- `style.css` — global styles and CSS custom properties (`--color-bg`, `--color-accent`, `--font-main`)
- `main.js` — ES module entry; imports GSAP and drives all animations

All HTML content, styling, and animation targets belong inside or attached to `#card`. GSAP is the sole animation dependency — do not introduce CSS `@keyframes` for motion that GSAP handles.

## Workshop Context

This repo is a starter template for a 30-minute design workshop. Participants use Claude to generate a personal name card by filling out a prompt template (see `name-card-workshop-playbook.md`). The design intent is that each person's card is unique — avoid hardcoding a single color scheme or layout in shared files.
