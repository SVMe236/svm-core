# SVM Core

A personal introduction website built as a first portfolio project. It shares a little about me, the things I'm interested in, and the ideas I try to live by, in a clean monochrome style. It comes in five languages and has a light and a dark mode.

## Live Demo

Visit the site: [svm-core.vercel.app](https://svm-core.vercel.app/)

## Features

- Personal introduction, interests, and personal philosophy sections
- **Five languages** with a flag-based language switcher:
  - English
  - العربية (Saudi Arabic, with full right-to-left layout)
  - Deutsch (written in a Bavarian-flavored German)
  - Русский
  - 한국어
- **Light and dark mode** with a circular reveal transition that grows from the toggle button
- Starts in the visitor's system theme, then remembers their theme and language choices
- Black, grey, and white visual theme
- Responsive layout for phones, tablets, and desktops
- Respects the "reduce motion" accessibility setting
- Lightweight static site with no build step and no dependencies

## Technologies

- HTML
- CSS (custom properties for theming)
- JavaScript (vanilla)
- Google Fonts (Noto Sans Arabic and Noto Sans KR, loaded only when needed)
- Vercel for deployment

## Run Locally

No build step is required. To view the site locally:

1. Download or clone this repository:

   ```bash
   git clone https://github.com/SVMe236/svm-core.git
   ```

2. Open the project folder.
3. Open `index.html` in your browser.

## Project Structure

```text
svm-core/
├── index.html     # Page, styles, scripts, and all translations
├── smolicon.ico   # Browser tab icon
└── README.md      # Project information
```

## Editing Translations

All translations live in one block inside `index.html` (the `<script type="application/json" id="i18n-data">` section near the bottom). Each language has the same set of keys, so to fix a word, find the key in that language and edit its text. Elements on the page are linked to these keys with `data-i18n` attributes.

To add a new language, copy an existing language block, translate the values, and add a matching option to the language menu and an entry to the `LANGS` list in the script.

## Deployment

This project is hosted on Vercel. The live site is available at [https://svm-core.vercel.app/](https://svm-core.vercel.app/). To publish your own changes, push them to the connected GitHub repository and Vercel will deploy the update.

## License

No license is specified for this project. Unless a license is added, all rights remain with the author; please ask before reusing or redistributing the project.
