# DDEV Playwright

DDEV Playwright is a DDEV addon that provides a simple way to run Playwright tests in your DDEV project.

## Getting started

```bash
# Install the ddev addon
ddev get thunder/ddev-playwright
# Install playwright at tests/Playwright
ddev install-playwright
# Restart ddev
ddev restart
# Run the tests
ddev playwright test
# Run the tests in UI mode
ddev playwright test --ui
# Show the latest report
ddev playwright show-report
```

### Access ddev website in tests

Add the following code to your playwright.config.js file:

```javascript
  use: {
    baseURL: process.env.PLAYWRIGHT_BASE_URL
  }
```

## Codegen

The codegen command is not supported yet. You can use [Playwright CRX](https://github.com/ruifigueira/playwright-crx) chrome extension instead.

