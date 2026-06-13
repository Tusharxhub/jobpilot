Overview

This repository will be organized following a professional full-stack layout used by senior engineers.

Recommended structure

- src/
  - server/ # API, server-only code, workers
  - client/ # Next.js pages, React components if split
  - shared/ # Types, utils used by both server & client
- config/ # runtime config, env schema, third-party configs
- infra/ # IaC (terraform, pulumi), DB migrations
- scripts/ # helper scripts (local dev, db tasks)
- docs/ # docs, architecture guides, onboarding
- public/ # static assets (existing)

Migration notes

- We'll scaffold `src/server` and `src/client` and migrate files in small, testable steps.
- Keep existing Next.js app in place until routes and imports are migrated.
- Prefer `src`-based imports (TypeScript `baseUrl`/paths) for clarity.

Next actions

1. Scaffold directories and starter files (done).
2. Update `package.json` scripts to support `dev`, `build`, `start`, `lint`, `format`.
3. Create a migration checklist and move files incrementally.

Guiding principles

- Keep changes minimal and incremental to avoid breaking production.
- Add clear docs for each migration step and update CI pipelines.
