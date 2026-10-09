# Vite Starter Template

A starter template for [bolt.diy](https://github.com/stackblitz-labs/bolt.diy).

## Purpose

This template is designed for use with **<https://github.com/stackblitz-labs/bolt.diy>**. bolt.diy fetches
these files at runtime and imports them into a fresh WebContainer project when you ask for a Vite + vanilla
JS/TS project, so everything here needs to install and build with no extra setup.

Modified by [Dustin Loring](https://github.com/Dustinwloring1988) (Dustinwloring1988) in October 2026.

## Stack

| Package | Version |
| --- | --- |
| Vite | ^8.3.4 |
| TypeScript | ~6.0.3 |

Node 20 or newer is required.

## Commands

```bash
npm install   # install dependencies
npm run dev   # vite — dev server
npm run build # vite build — production build
npm run preview # vite preview — local preview server
```

## About this template

A minimal Vite project with no frameworks pre-installed. Edit `main.js` or add your own entry point.
The `vite.config.ts` is configured for fast refresh and production optimization.

## Upgraded to Vite 8 (October 2026)

Moved from Vite 5. The upgrade stepped through Vite 6 and Vite 7, with `npm install` verified after each
step. The final state has Vite 8.3.4 with TypeScript ~6.0.3.

TypeScript is on 6.x rather than 7 because the Vite ecosystem caps TS (`svelte-check ^5||^6`,
`typescript-eslint <6.1.0`). Exception: some templates ship TS 7.0.2 with bare `tsc` and no checker
constraint.

A `.gitignore` was added as part of the Vite 6 migration. The template previously had none, which also
blocked `npm install` on a dirty working tree.

## Verification

- `npm install` and `npm run build` pass
- Confirmed the dev server starts and HMR works
- `npm run preview` serves the production build locally