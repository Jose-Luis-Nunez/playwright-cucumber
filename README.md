# Playwright Cucumber example project
![main](https://github.com/Jose-Luis-Nunez/playwright-cucumber/actions/workflows/run_tests.yml/badge.svg?branch=main)

example frontend automation project with Playwright in JS with cucumber
### before starting
1 `npm install`

2 `npx playwright install `
### Run tests
`npm run test`

### Example test with cucumber
```gherkin
Feature: Check24 Main Page

  Scenario: Search for Products
    Given I open Check24 page
    When I search for "PS5"
    Then I am on product result page
```

### headless false
the test will run headless,to see a browser change the value in the "GlobalHooks.js" to false
`this.browser = await chromium.launch({ headless: false });`
