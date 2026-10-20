# Demo Notes — Copilot Pipeline Walkthrough

This document outlines the end-to-end walkthrough rehearsed for the hands-on session.

## What the walkthrough covers

1. **Greenfield repository** — a fresh repo, initialized with a README, is the starting point.
2. **Issues as the source of truth** — work is planned as issues (e.g. #1 CONTRIBUTING guidance, #2 the session checklist).
3. **Copilot coding agent pickup** — an issue is assigned to the Copilot coding agent, which can open a draft PR with the proposed changes.
4. **Line-anchored PR review** — an inline review comment is attached to a specific line of the diff, referencing the `CI Pipeline` job.
5. **CI actually running** — the `CI Pipeline` workflow (`.github/workflows/ci.yml`) triggers on push and manual dispatch, checks out the code, and echoes a greeting.
6. **Security hygiene** — a check for repository security advisories rounds out the session.

## Tips for the live demo

- Keep the PR diff small so the line-anchored comment lands cleanly.
- Trigger the workflow manually via workflow dispatch so the run is easy to find.
- Submit your own review as a plain comment, not an approval, since you cannot approve your own PR.
