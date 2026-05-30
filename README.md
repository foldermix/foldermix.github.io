# foldermix.github.io

[![Website](https://img.shields.io/badge/site-foldermix.github.io-1f6feb)](https://foldermix.github.io)
[![Built with Astro](https://img.shields.io/badge/built%20with-Astro-ff5d01)](https://astro.build/)
[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

Product website for [foldermix](https://github.com/foldermix/foldermix), the open-source tool that packs a folder into one LLM-ready context file for ChatGPT, Claude, Gemini, and other assistants.

Created by [Shay Palachy Affek](http://www.shaypalachy.com/).

Live site: [foldermix.github.io](https://foldermix.github.io)

## What This Repo Contains

This repository contains the public foldermix landing site. It introduces the three user-facing ways to use foldermix:

| Surface | Purpose | Link |
|---|---|---|
| CLI | Scriptable local packing for developers and agents | [foldermix/foldermix](https://github.com/foldermix/foldermix) |
| Desktop | Native macOS app for point-and-click packing | [foldermix/foldermix-desktop](https://github.com/foldermix/foldermix-desktop) |
| Web | Browser-based packing for zipped folders | [foldermix.shaypalachy.com](https://foldermix.shaypalachy.com) |

The site is intentionally small: a polished product homepage, a redirect from `/web/` to the hosted web app, shared layout metadata, and static icons.

## Local Development

Requirements:

- Node.js 22.12 or newer
- npm

Install dependencies:

```sh
npm install
```

Start the development server:

```sh
npm run dev
```

Astro serves the site at `http://localhost:4321` by default.

## Build and Preview

Build the production site:

```sh
npm run build
```

Preview the built output locally:

```sh
npm run preview
```

The static build is written to `dist/`.

## Project Structure

```text
.
├── public/
│   ├── favicon.ico
│   └── favicon.svg
├── src/
│   ├── layouts/
│   │   └── Base.astro
│   └── pages/
│       ├── index.astro
│       └── web.astro
├── astro.config.mjs
├── package.json
└── tsconfig.json
```

Key files:

- `src/pages/index.astro` - the product homepage for CLI, desktop, and web.
- `src/pages/web.astro` - redirects `/web/` to the hosted foldermix web app.
- `src/layouts/Base.astro` - shared HTML head, metadata, and global styling.

## Related Repositories

- [foldermix/foldermix](https://github.com/foldermix/foldermix) - CLI, library, and core documentation.
- [foldermix/foldermix-desktop](https://github.com/foldermix/foldermix-desktop) - macOS desktop app.

## License

This website source is released under the [MIT License](LICENSE).

## Credits

Created by [Shay Palachy Affek ](http://www.shaypalachy.com/) [[GitHub](https://github.com/shaypal5)]
