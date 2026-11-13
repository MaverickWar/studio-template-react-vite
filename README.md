# Studio template: React (Vite)

The starter Universal App Studio copies when someone picks **Vite + React + TypeScript** while setting up a new project.

It's the official `npm create vite@latest -- --template react-ts` starter, plus one change: **the look comes from `design/tokens.json`**.

- `design/tokens.json` holds the colours, fonts, corners and spacing. Studio replaces it with the project's own design straight after copying this template.
- `design/adapters/web/studio-theme.ts` turns those tokens into `--studio-*` CSS variables and loads the two fonts. `src/main.tsx` calls `applyTheme()` once.
- Style everything with the variables (`var(--studio-primary)` and so on). Change the look in Studio, never by typing colours into the code.

## Running it

```
npm install
npm run dev
```

Open http://localhost:5173.

## Checks

```
npm run lint
npm run build
npm test
```

The same checks run on GitHub for every push and pull request (`.github/workflows/checks.yml`).
