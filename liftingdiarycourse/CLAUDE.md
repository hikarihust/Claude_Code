# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Lifting Diary Course — a Next.js 16 web application built with React 19, TypeScript, and Tailwind CSS 4. Uses the App Router pattern (`src/app/`).

## Commands

- `npm run dev` — Start development server
- `npm run build` — Production build
- `npm run start` — Start production server
- `npm run lint` — Run ESLint (flat config with core-web-vitals + typescript rules)

No test framework is configured yet.

## Architecture

- **Routing:** Next.js App Router — pages live in `src/app/`, each folder = route segment
- **Styling:** Tailwind CSS 4 via `@tailwindcss/postcss` plugin; global theme variables in `src/app/globals.css`
- **Fonts:** Geist sans and mono loaded via `next/font` in `src/app/layout.tsx`, exposed as CSS variables
- **Path alias:** `@/*` maps to `./src/*` (configured in tsconfig.json)
- **TypeScript:** Strict mode enabled, target ES2017
