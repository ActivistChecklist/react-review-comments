# Agent Instructions

- Always use the Changesets process for version bumps (create a changeset and run versioning via Changesets), never manual version edits.
- Every releasable change must include a `.changeset/*.md` file; do not rely on version/package edits alone.
- This repo uses **pnpm** (pinned via `packageManager` in `package.json`). Use `pnpm install --frozen-lockfile`, and commit `pnpm-lock.yaml`; do not add a `yarn.lock` or `package-lock.json`.
