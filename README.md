# vocab.ai

vocab.ai is a single-purpose vocabulary revision web app for SSC CGL aspirants.

## Goal

A user enters an English word or phrase. The app returns:

- Hindi meaning
- Two synonyms
- Two antonyms
- One SSC CGL-style example sentence
- Hindi meaning of the example sentence

Every generated entry is saved in the learner's browser so it can be revised later and downloaded as a PDF.

## Target user

SSC CGL aspirants who want quick English vocabulary practice with Hindi support.

## Live site

After GitHub Pages is enabled, the site is available at:

```text
https://hellosamar.github.io/vocab.ai/
```

Repository:

```text
https://github.com/HelloSamar/vocab.ai
```

## Files kept in this repository

```text
index.html
README.md
.github/workflows/pages.yml
.nojekyll
```

Everything unrelated to the vocabulary app has been removed from the active `main` branch.

## Features

- SSC CGL-focused vocabulary lookup
- Hindi meaning for the searched word or phrase
- Two synonyms and two antonyms
- SSC-style example sentence
- Hindi meaning of the example sentence
- Local revision history using `localStorage`
- Download saved revision list as PDF
- Download saved revision list as JSON backup
- Clear saved history
- Works as a static GitHub Pages site

## Data storage

Saved lookups are stored locally in the user's browser with `localStorage`. They are not stored on a server.

## Deployment

GitHub Pages deployment is handled by:

```text
.github/workflows/pages.yml
```

Use GitHub repo settings if needed:

```text
Settings -> Pages -> Source -> GitHub Actions
```

## Note about accuracy

This is a static frontend app. It uses built-in SSC-style examples for common exam words and public browser-side lookup services where available. For perfect AI-quality results for every phrase, connect a small backend API later.
