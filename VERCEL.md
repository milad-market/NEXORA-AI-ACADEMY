# Vercel deployment notes

This repository intentionally uses the Next.js Pages Router fallback. The production entrypoint is `pages/index.tsx` and must be at the repository root selected by Vercel.

Before deploying, verify that Vercel Project Settings -> Build & Deployment -> Root Directory is the repository root (`./`) and that GitHub commit contains `pages/index.tsx` and `package.json` at that same level.

Commands:
- npm ci
- npm run typecheck
- npm test
- npm run build

Never upload the ZIP file itself as the application source. Extract it and commit its contents at repository root.
