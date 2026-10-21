# TanStack Start + FSD

React full-stack starter based on [TanStack Start](https://tanstack.com/start), organized with [Feature-Sliced Design](https://fsd.how/).

## Table of contents

- [Stack](#stack)
  - [Framework & routing](#framework--routing)
  - [Builder & language](#builder--language)
  - [UI](#ui)
  - [Architecture](#architecture)
  - [Quality & tests](#quality--tests)
- [Getting started](#getting-started)
- [Scripts](#scripts)
- [Structure](#structure)

## Stack

### Framework & routing

- [React](https://react.dev/)
- [TanStack Start](https://tanstack.com/start)
- [TanStack Router](https://tanstack.com/router)

### Builder & language

- [Vite](https://vite.dev/)
- [TypeScript](https://www.typescriptlang.org/docs/)
- [pnpm](https://pnpm.io/)

### UI

- [Tailwind CSS](https://tailwindcss.com/docs)
- [shadcn/ui](https://ui.shadcn.com/)
- [Base UI](https://base-ui.com/)
- [class-variance-authority](https://cva.style/docs)
- [Lucide](https://lucide.dev/guide/packages/lucide-react)
- [Inter (Fontsource)](https://fontsource.org/fonts/inter)

### Architecture

- [Feature-Sliced Design](https://fsd.how/)
- [@feature-sliced/cli](https://github.com/feature-sliced/cli)

### Quality & tests

- [Biome](https://biomejs.dev/guides/getting-started/)
- [Steiger](https://github.com/feature-sliced/steiger)
- [Vitest](https://vitest.dev/)
- [Playwright](https://playwright.dev/)

## Getting started

```bash
pnpm install
pnpm dev
```

App runs at [http://localhost:3000](http://localhost:3000).

## Scripts

| Command | Purpose |
| --- | --- |
| `pnpm dev` | Dev server |
| `pnpm build` | Production build |
| `pnpm check` | Biome lint + format |
| `pnpm lint:fsd` | FSD lint (Steiger) |
| `pnpm lint:all` | Biome + Steiger |
| `pnpm fsd` | Scaffold FSD layers/slices ([CLI](https://github.com/feature-sliced/cli)) |
| `pnpm test` | Unit tests (Vitest) |
| `pnpm test:e2e` | E2E tests (Playwright) |

## Structure

```text
src/
  app/       # App init, TanStack routes, styles
  pages/     # Pages (FSD slices)
  shared/    # UI kit, utils (no business logic)
e2e/         # Playwright tests
```
