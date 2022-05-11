# [12DaysOfCoding](admin/team.md)
[![CI](https://github.com/12DaysOfCoding/WeTheFoodies/actions/workflows/main.yml/badge.svg)](https://github.com/12DaysOfCoding/WeTheFoodies/actions)
[![CD](https://github.com/cse110-fa21-group30/cse110-fa21-group30/actions/workflows/firebase-hosting-merge.yml/badge.svg)](https://cse110-group30-affd4.web.app/)
[![Codacy](https://github.com/12DaysOfCoding/WeTheFoodies/actions/workflows/codacy-analysis.yml/badge.svg)](https://github.com/12DaysOfCoding/WeTheFoodies/actions)

## Project Description
Our team will design a recipe management application.

## Setup Instructions
1. ```git clone https://github.com/cse110-fa21-group30/cse110-fa21-group30.git```
2. Get [nodejs](https://nodejs.org/en/download/) if you don't already have.
3. In the root dir of this project, run `npm install`. This will install [ESLint](https://eslint.org/) and [Jest](https://jestjs.io/).
4. To run the linter, do `npm run lint`. Only unfixable problems will be reported.
5. To run unit tests, `npm run test`
6. To run e2e tests, `npm run e2e`

## Contribution
1. Make changes in the folder called `source`, more specifically, the `html` files are placed directly inside the `source` while the `css` and `js` files are placed inside `assets/style` and `assets/scripts` respectively.
2. Run `npm run lint` to lint the code up to standard.
3. Follow the [testing writeup](#testing), add more unit and end to end tests to the corresponding folder (highly recommended).
4. Run `npm run test` to execute unit tests. Fix any issue.
5. Run `npm run e2e` to execute end to end test. Fix any issue.
6. Commit all changes and push.
7. Make a pull request and fill out the template. Request some reviews.
8. Make sure all status checks are passed before merging

## Testing
* We are using a combination of [Jest](https://jestjs.io/) and [puppeteer](https://developers.google.com/web/tools/puppeteer) to run tests.
* Jest is for unit tests and puppeteer is for end to end tests.
* Note there is a folder call `/tests` in the root dir. Within this folder, you have one folder called `unit` and another called `e2e`. Each contains an example of how to write a simple test.

## [Documentation](https://cse110-fa21-group30.github.io/cse110-fa21-group30/)
This is auto generated by [JSDoc](https://jsdoc.app/about-getting-started.html)
You need to follow their guideline (preceding functions with a line or block comment) in order for the documentation to show up.
Ex.
```
/**
 * returns the sum of a and b
 * @param {int} a - first number
 * @param {int} b - second number
 */
const add = (a, b) => a + b;
```

## Linting 
- Ideally, make sure to lint locally before make the pull request. But it's fine to just push to repo, since CI pipeline would lint again just in case. 
- We are using [ESLint](https://eslint.org/) as linter. 
- Only files within the "src" directory would be linted. 

## Quality analysis automation
- We are using [Codacy](https://www.codacy.com/) to analysis the quality of the source code. 
- For each pull request, the CI/CD pipeline ([this file in particular](.github/workflows/codacy-analysis.yml)) would automatically enable Codacy and perform analysis as needed. 
- Codacy also provided us the dashboard to monitor various aspects of the project, including code duplication, complexity, etc. 
