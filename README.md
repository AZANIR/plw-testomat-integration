# Playwright tests with testomat integration


## Table of Contents

- [Description](#description)
- [Structure](#structure)
- [Composition](#composition)
- [Configuration](#configuration)
- [Usage](#usage)
- [Running setup](#running-setup)
- [Test structure](#test-structure)
- [Reports](#reports)

### Description

Single repository for tests automation of the CreditOnline project

### Structure

- Folders:
    - playwright-report: Contains results and reports of tests runs
    - node_modules: Contains node.js modules needed to run tests
    - test: Contains pageFactory and specs folders
        - pageFactory: Contains pageFactory files with reusable testing functions
        - specs: Contains test files organized by modules and structure

- Files:
    - .gitignore: Excludes files and folders from uploading to GitHub
    - playwright.config.ts: Contains settings for the playwright test runner
    - LICENSE: Contains the text of the project's license
    - package.json: Contains project data and dependencies
    - package-lock.json: Contains fixed project dependencies for quick installation
    - readme.md: Contains a description and brief documentation of the project

### Composition

- Dependencies:
    - playwright
    - testomatio

### Configuration

Config files contain settings to run tests with different parameters and settings in different browsers. 

### Usage

```bash
export TESTOMATIO=your-api-key && npx playwright test --config=playwright.config.ts
```


### Running setup

Scripts are available to automate common tasks in the project. 
### Test structure

The tests are organized using describe and test blocks. Each test block represents a specific test case. 

### Reports

Test reports can be generated in folder playwright-report. And can be viewed in the browser. Also in the dashboard of the testomat.io service.

![Testomat.io](https://i.imgur.com/ejXFbs9.png)
