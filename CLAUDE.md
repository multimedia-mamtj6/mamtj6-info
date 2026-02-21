# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static personal/business website hosted on GitHub Pages at `info.mamtj6.com` (configured via `CNAME`). There is no build system, bundler, or package manager — all files are plain HTML, CSS, and JavaScript served directly.

## Architecture

- **`index.html`** — Root landing page (currently placeholder text)
- **`contact/admin.html`** — A self-contained interactive digital business card with:
  - 3D tilt effect on mouse hover (vanilla JS)
  - Click-to-flip card animation (CSS 3D transforms)
  - Front face: logo, org name, employee name, job title
  - Back face: QR code, contact info links, social links, vCard download button
  - `.no-flip` class on interactive elements prevents flip when clicking links/buttons
  - All CSS is inline (in `<style>` tag), all JS is inline (in `<script>` tag)
  - Uses Google Fonts (Poppins) and FontAwesome 6.4.0 via CDN
  - CSS variables defined in `:root` for theming (`--accent-green`, `--accent-blue`, etc.)
- **`media/background/pattern.svg`** — Islamic geometric pattern SVG used as a background asset

## Development

No build or test commands. To develop locally, open HTML files directly in a browser or use any static file server (e.g., `npx serve` or VS Code Live Server extension).

## Deployment

Pushes to `main` branch deploy automatically via GitHub Pages.
