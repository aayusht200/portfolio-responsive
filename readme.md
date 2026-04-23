# Responsive Portfolio

A personal portfolio site built with plain HTML, CSS, and JavaScript, bundled with Webpack.

The current project focuses on a responsive landing page with:

- an intro / about section
- social profile links
- a project showcase grid
- a contact section
- tablet and mobile layout adjustments

## Tech Stack

- JavaScript
- HTML
- CSS
- Webpack 5
- Babel
- Biome
- Jest

## Project Structure

```txt
portfolio-responsive/
├── assets/
│   └── headshot.png
├── src/
│   ├── index.js
│   ├── style.css
│   └── template.html
├── babel.config.cjs
├── biome.json
├── package.json
├── webpack.dev.js
├── webpack.prod.js
└── readme.md
```

## Getting Started

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm start
```

Create a production build:

```bash
npm run build
```

## Available Scripts

- `npm start` runs the webpack dev server
- `npm run build` creates the production bundle in `dist/`
- `npm run lint` checks the codebase with Biome
- `npm run format` applies Biome fixes
- `npm run lint-format` runs Biome with write mode
- `npm run test` runs Jest
- `npm run test:watch` runs Jest in watch mode

## Current Implementation Notes

- The app entry point is `src/index.js`
- The page markup lives in `src/template.html`
- Styling and responsive breakpoints live in `src/style.css`
- Image assets are handled by Webpack asset modules
- The site currently uses a local headshot image plus CDN-hosted social icons

## Deployment

This repo includes GitHub Pages helper scripts:

```bash
npm run deploy
npm run reset
```

These scripts assume a `main` branch and a `gh-pages` deployment flow.

## Next Content Updates

The portfolio structure is in place, but some content is still placeholder content. Good next updates would be:

- replace the lorem ipsum bio and project descriptions
- add real project names and live links
- update the contact details in the footer
- add tests if interactive JavaScript is introduced later
