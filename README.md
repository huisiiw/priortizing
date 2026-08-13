# Priortizing

A quiet AI task organizer. Dump everything first; GLM turns the note into a small, stable action view when you are ready.

## [Open the live demo →](https://huisiiw.github.io/priortizing/)

## What it does

- Captures tasks as naturally as writing in Apple Notes
- Uses Zhipu AI's `glm-4.7-flash` to understand, classify, and prioritize tasks
- Extracts explicit Chinese dates and relative times without inventing deadlines
- Keeps manual ordering, category names, and user overrides authoritative
- Falls back to a local organizer if the model or network is unavailable
- Installs as a PWA and keeps task data in the browser

## Architecture

`GitHub Pages PWA → secure server route → Zhipu GLM API`

The model key is stored as an encrypted server-side secret and is never shipped to the browser or committed to GitHub. Model responses pass strict structural and task-ID validation before reaching the interface.

## Project status

Working AI-enabled PWA prototype, built as a portfolio project.
