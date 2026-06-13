Migration checklist

- [ ] Add `src/shared` for common types and utils
- [ ] Add path aliases in `tsconfig.json`
- [ ] Move `lib/` utilities to `src/shared` or `src/server` as appropriate
- [ ] Move API routes incrementally and update route imports
- [ ] Ensure `public/` remains the canonical static folder
- [ ] Update CI to build from `src/` if needed
