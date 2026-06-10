# Hortora engine — Project Handoff

*Last updated: 2026-06-08*

---

## What's In Flight

Branch `issue-3-multi-domain-filter` (pushed, not yet merged):
- Closes #3: `?domain=jvm&domain=tools` multi-domain filter via `IsIn`
- Closes #4: SearchResource refactor — `doSearch()` extracted, unchecked cast removed, `parseCurationScore` renamed

PR creation pending — branch is pushed to origin, no PR opened yet.

## Immediate Next Step

Open a PR for `issue-3-multi-domain-filter` → main, then merge.

## What's Next

| # | Description | Scale | Complexity |
|---|-------------|-------|------------|
| — | Phase 2 design: SPLADE + cross-encoder reranker | L | High | Gated on casehubio/onnx-inference prototype |
| — | Federation: canonical/child chain walk | M | Med | Hortora-specific, no shared module |
| — | Incremental re-indexing / file watching | S | Med | Startup-only currently |

## Key References

| Resource | Location |
|---|---|
| engine spec | `docs/DESIGN.md` |
| Phase 2 spec | `casehubio/onnx-inference` design doc |
| Open issues | `gh issue list --repo Hortora/engine` |
