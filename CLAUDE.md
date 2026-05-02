# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Running locally

Open `index.html` directly in a browser — no build step, no dependencies, no server required.

The live site is at https://aimeemalan.github.io/aimee-malan-personal-homepage (deployed via GitHub Pages from the `main` branch).

## Architecture

The entire site is a single `index.html` file. All CSS is written inline in a `<style>` block in `<head>` — there are no external stylesheets. JavaScript is not used. The photo is `images/photo.jpg` and the favicon is `favicon.svg`.

**CSS design tokens** are defined as CSS custom properties at `:root` (`--black`, `--white`, `--gray-100/300/500/700`). All colors reference these variables.

**Fonts** are loaded from Google Fonts: EB Garamond (serif, used for headings and the nav name) and Inter (sans-serif, used for body text).

**Page sections** (in order): sticky nav → hero (photo + intro) → about → experience → education → contact. Each section has an `id` matching the nav anchor links.

**Responsive layout** is handled with a single CSS media query breakpoint.
