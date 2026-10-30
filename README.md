# PW_TS

End-to-end tests built with [Playwright](https://playwright.dev/) and TypeScript. Tests run on Chromium.

## Setup

Requires Node.js (LTS).

```sh
npm ci
npx playwright install --with-deps chromium
```

## Running tests

```sh
# All tests
npx playwright test

# One test
npx playwright test tests/example.spec.ts -g "has title" --reporter=line

# Open the HTML report
npx playwright show-report
```

## Project layout

- `tests/` – test specs
- `playwright.config.ts` – Playwright configuration
- `.github/workflows/playwright.yml` – CI, runs on pushes and pull requests to `main`/`master`

## License

[MIT](LICENSE)
