# PW_TS

Playwright 1.64 + TypeScript, npm. Chromium project only. Specs live in `tests/`; config in `playwright.config.ts`.

## Commands
- All tests: `npx playwright test`
- One test: `npx playwright test <file> -g "<name>" --reporter=line`
- Report: `npx playwright show-report`

## Conventions
- Import from `@playwright/test`.
- Prefer role-based locators and web-first assertions (`await expect(...)`).

## Working style
- Search for the target first; read only relevant files, and don't re-read unchanged ones.
- Keep diffs minimal; no unrelated refactors.
- Keep replies concise unless detail is requested.
- Run only the specs affected by a change, with `--reporter=line`; trim long command output.
- Skip subagents for small tasks.
- Ask before destructive operations.
