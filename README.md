# NEXORA AI ACADEMY

Premium Persian-first interactive AI education platform built with Next.js.

## Features
- Persian/English UI with RTL/LTR
- Adaptive curriculum, searchable lessons, local progress persistence
- AI Teacher with OpenAI, Gemini, and Anthropic adapters via server-side API
- Multi-AI comparison endpoint when multiple credentials are configured
- Prompt Lab
- Interactive AI Lab visualizations
- Quiz engine with real local scoring
- AI glossary
- Project Workshop
- Premium Liquid Glass UI + Theme Studio presets
- PWA manifest + service worker
- Reduced-motion support and responsive layouts

## Environment
Copy `.env.example` to `.env.local` and set only the providers you actually have credentials for.

- `OPENAI_API_KEY`
- `OPENAI_MODEL`
- `ANTHROPIC_API_KEY`
- `ANTHROPIC_MODEL`
- `GOOGLE_GENERATIVE_AI_API_KEY`
- `GEMINI_MODEL`

Secrets are server-side only.

## Commands
`npm install`
`npm run typecheck`
`npm test`
`npm run build`
`npm start`

## Honest limitations
The Python Playground intentionally does not execute arbitrary Python on the server. A production sandbox should use an isolated WASM runtime or dedicated sandbox service. AI features show unavailable state when no real provider credential is configured.

UI/UX Pro Max was not available as an installed skill in this environment, so the Liquid Glass design system was implemented manually and this limitation is documented here.
