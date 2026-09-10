# Personal Portfolio

My personal portfolio, built with Next.js, React, TypeScript, and Tailwind CSS.

## What's here

- A terminal-inspired design with an animated introduction and canvas matrix rain
- An about page with my background, development philosophy, and skills
- Project cards with demo and source links, plus write-ups for Minesweeper and Pakudex
- Cal.com booking at `/hire-me` and a Formspree contact form at `/hire-me/email`
- Responsive layouts and reduced-motion support
- Vercel Analytics and Speed Insights

## Running locally

The Node version is recorded in `.nvmrc`. With nvm installed:

```sh
nvm use
npm ci
npm run dev
```

Open [localhost:3000](http://localhost:3000). To build and run the production version:

```sh
npm run build
npm start
```

## Editing the site

| What to change                        | Where                                                          |
| ------------------------------------- | -------------------------------------------------------------- |
| Project entries                       | `src/app/projects/page.tsx`                                    |
| Project card layout and fields        | `src/components/core/project-card.tsx`, `src/types/project.ts` |
| Project images                        | `public/project-icons/`                                        |
| Homepage introduction                 | `src/components/core/hero-section.tsx`                         |
| About text                            | `src/app/about/page.tsx`                                       |
| Colors and shared styles              | `tailwind.config.ts`, `src/app/globals.css`                    |
| Navigation, booking, and contact form | `src/components/core/`                                         |

The homepage project count is hardcoded. Update it when adding or removing projects.

## Known gaps

- `npm run lint` calls `next lint`, which is unavailable in the installed Next.js CLI. The script needs updating.
- `.npmrc` enables `legacy-peer-deps`, originally added for a Formspree and React 19 compatibility issue. Its current necessity has not been checked.

Planned work lives in [GitHub issues](https://github.com/Eric-Zhang-Developer/personal-portfolio/issues). Agent working instructions live in [AGENTS.md](AGENTS.md).
