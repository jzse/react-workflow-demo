# react-workflow-demo

[![Build Status][travis-svg]][travis-url]
[![NPM dependency status][david-dep-svg]][david-dep-url]
[![NPM dev dependency status][david-dev-dep-svg]][david-dev-dep-url]

Demo for a simple `create-react-app` app development workflow.

* [Live site][project-url] is deployed from the master branch
  * Travis CI tests, builds and deploys to GitHub Pages
  * Netlify creates a mirror build and deploys to its own platform
* Changes are made by pull request
  * Netlify will build the branch and deploy to a [deploy preview URL](https://deploy-preview-3--jzse.netlify.com/) for review
* Better quality code commits
  * [lint-stage](https://github.com/okonet/lint-staged): allow only properly formatted JS to be committed
  * [husky](https://github.com/typicode/husky): run npm scripts (lint-stage) on any git hook
  * [commitizen](https://github.com/commitizen/cz-cli): provide commit message template options when using `npm run commit` in place of `git commit`

## Quickstart

```sh
# Demo the site
git clone git@github.com:jzse/react-workflow-demo.git
cd react-workflow-demo
npm run start
```


[project-url]: https://jzse.github.io/react-workflow-demo
[travis-svg]: https://travis-ci.org/jzse/react-workflow-demo.svg
[travis-url]: https://travis-ci.org/jzse/react-workflow-demo
[david-dep-svg]: https://david-dm.org/jzse/react-workflow-demo.svg
[david-dep-url]: https://david-dm.org/jzse/react-workflow-demo
[david-dev-dep-svg]: https://david-dm.org/jzse/react-workflow-demo/dev-status.svg
[david-dev-dep-url]: https://david-dm.org/jzse/react-workflow-demo?type=dev
