# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static GitHub Pages website for an artist portfolio (Madzia Zalewa). It's a simple static site with no build system - files are served directly.

## Development

To develop locally, serve the files with any static HTTP server:
```bash
python3 -m http.server 8000
# or
npx serve .
```

Then open http://localhost:8000 in a browser.

## Architecture

- **Main site** (`/index.html`): Artist portfolio built on the Nevada Bootstrap template (Bootstrap 3). Uses jQuery for interactions, Bootstrap carousel for image slider, and modal gallery for portfolio viewing.
- **Puzzle** (`/puzzle/`): Interactive jigsaw puzzle game (from CodePen by Dillo). Self-contained with its own `script.js`, `style.css`, and assets (`img/`, `audio/`).

## Key Files

- `css/style.css` - Main site custom styles (modify this, not bootstrap.css)
- `js/script.js` - Main site custom JavaScript
- `puzzle/script.js` - Puzzle game logic (canvas-based, touch-compatible)

## Template Attribution

Main site based on Nevada template by Nicola Tolin (Apache 2.0 license).
