# CLAUDE.md

A developer knowledge hub for snippets, commands, prompts, notes, files, images, links and custom types.

## Context Files

Read the following to get the full context of the prject:

- @context/project-overview.md
- @context/coding-standars.md
- @context/ai-interaction.md
- @context/current-feature.md

## Commands

```bash
npm run dev      # Start dev server at http://localhost:3000
npm run build    # Production build
npm run lint     # Run ESLint
```

## Stack

- **Next.js 16** with App Router (`src/app/`)
- **React 19** with React Compiler enabled (`reactCompiler: true` in `next.config.ts`)
- **TypeScript**
- **Tailwind CSS v4** (via `@tailwindcss/postcss`)

## Architecture

Uses the Next.js App Router convention — routes map to folders under `src/app/`. Layouts wrap pages via `layout.tsx`. No pages router.

The React Compiler is enabled, so avoid manual `useMemo`/`useCallback` optimizations — the compiler handles them automatically.
