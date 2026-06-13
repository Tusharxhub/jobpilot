Refactor Plan (incremental)

1. Inventory: list modules, pages, API routes, and shared utilities.
2. Create `src/server`, `src/client`, `src/shared` and update TS `paths`.
3. Move server-only utilities and API routes into `src/server` one folder at a time.
4. Move UI components into `src/client` and keep `app/` working until migration completes.
5. Run tests and typecheck after each small move; revert if errors appear.
6. Clean up root-level files and update imports and build configs.

Safety rules

- Do not move files that are required by Next.js runtime without updating imports.
- Use feature branches and small PRs for each module migration.
