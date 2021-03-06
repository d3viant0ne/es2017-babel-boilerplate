## ES7+ Babel driven library boilerplate
[![test][test]][test-url] [![coverage][cover]][cover-url] [![quality][quality]][quality-url] [![issues][issues]][issues-url]


#### Contents
- [Features](#Features)
- [Usage](#usage)
- [Testing](#testing)
- [Performance Benchmarks](#benchmarking-suite)
- [Security](#security)


#### Features
- ES6 / ES7 transpilation with [Babel][babel-url]
- ES6+ minification with Babili [babili][babili-url]
- ES6+ Testing via [babel-register][babel-register-url] with [Mocha][mocha-url] & [Chai][chai-url]
- HTML Test Reports via [mochawesome][mochawesome-url]
- Code Linting with [ESLint][eslint-url]
- Benchmark Testing with [benchmark.js][benchmark-url]
- Code monitoring and auto server restart with [nodemon][nodemon-url]
- Security vulnerability scan with [nsp][nsp-url]
- Docker build for non-lib projects.

#### Usage

- `npm start` - execute code in `src` directory with live reload via `nodemon` transpiled with `babel-node`
- `npm run serve:dev <target>` - execute target code with live reload via `nodemon` transpiled with `babel-node`
- `npm run benchmark` - run benchmark tests with `benchmark.js`
- `npm run benchmark:watch` - run benchmark tests with `benchmark.js` and watch for file changes
- `npm run lint` - code linting with `eslint`
- `npm run lint:fix` - fix problems automatically with `eslint`
- `npm test` - run tests with `mocha` and `chai` with spec as reporter and `nyc` code coverage
- `npm run test:watch` - run tests with `mocha` and `chai` and watch for changes
- `npm run test:report` - export tests results as html files in the `./reports` folder via `mochasome`
- `npm run build:dist` - transpile and minify ES6+ code and create sourcemaps with `babel` & `babili`
- `npm run serve:dist` - serve production files from the `./dist` folder via `node`
- `npm run scan:security` - run vulnerability tests via the node security platform `nsp`

#### Testing

_Testing with [Mocha][mocha-url] and [Chai][chai-url], HTML Reports via [mochawesome][mochawesome-url]_

```bash
npm test

```

#### Benchmarking Suite

_Benchmark Testing with [Benchmark.js][benchmark-url]_

```bash
npm run benchmark

```

#### Security

_Run vulnerability tests via `Node Security Project`_


[test]: https://travis-ci.org/d3viant0ne/es2017-babel-boilerplate.svg?branch=master
[test-url]: https://travis-ci.org/d3viant0ne/es2017-babel-boilerplate
[cover]: https://codecov.io/gh/d3viant0ne/es2017-babel-boilerplate/branch/master/graph/badge.svg
[cover-url]: https://codecov.io/gh/d3viant0ne/es2017-babel-boilerplate
[quality]: https://www.bithound.io/github/d3viant0ne/es2017-babel-boilerplate/badges/score.svg
[quality-url]: https://www.bithound.io/github/d3viant0ne/es2017-babel-boilerplate
[issues]: https://www.bithound.io/github/d3viant0ne/es2017-babel-boilerplate/badges/devDependencies.svg
[issues-url]: https://www.bithound.io/github/d3viant0ne/es2017-babel-boilerplate/master/dependencies/npm
[babel-url]: https://github.com/babel/babel
[babili-url]: https://github.com/babel/babili
[babel-register-url]: https://github.com/babel/babel/tree/master/packages/babel-register
[mocha-url]: https://github.com/mochajs/mocha
[chai-url]: https://github.com/chaijs/chai
[mochawesome-url]: https://github.com/adamgruber/mochawesome
[eslint-url]: https://github.com/eslint/eslint
[benchmark-url]: https://github.com/bestiejs/benchmark.js
[nodemon-url]: https://github.com/remy/nodemon
[nsp-url]: https://github.com/nodesecurity/nsp
