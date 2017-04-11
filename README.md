# test coverage for  [ramda (v0.23.0)](http://ramdajs.com/)  [![npm package](https://img.shields.io/npm/v/npmtest-ramda.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-ramda) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-ramda.svg)](https://travis-ci.org/npmtest/node-npmtest-ramda)
#### A practical functional library for JavaScript programmers.

[![NPM](https://nodei.co/npm/ramda.png?downloads=true)](https://www.npmjs.com/package/ramda)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-ramda/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-ramda/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-ramda/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-ramda/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-ramda/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-ramda/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-ramda/tree/gh-pages/build)|

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-ramda/build/screenCapture.buildCustomOrg.browser.coverage.html.png)](https://npmtest.github.io/node-npmtest-ramda/build/coverage.html/index.html)

[![test-report](https://npmtest.github.io/node-npmtest-ramda/build/screenCapture.buildCustomOrg.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmtest%252Fnode-npmtest-ramda%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-ramda/build/test-report.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-ramda/build/screenCapture.buildApidoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-ramda%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-ramda/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-ramda/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-ramda/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Scott Sauyet",
        "email": "scott@sauyet.com",
        "url": "scott.sauyet.com"
    },
    "bugs": {
        "url": "https://github.com/ramda/ramda/issues"
    },
    "contributors": [
        {
            "name": "Michael Hurley",
            "email": "mh@buzzdecafe.com",
            "url": "http://buzzdecafe.com"
        },
        {
            "name": "Scott Sauyet",
            "email": "scott@sauyet.com",
            "url": "http://fr.umio.us"
        },
        {
            "name": "David Chambers",
            "email": "dc@davidchambers.me",
            "url": "http://davidchambers.me"
        },
        {
            "name": "Graeme Yeates",
            "email": "yeatesgraeme@gmail.com",
            "url": "https://github.com/megawac"
        }
    ],
    "dependencies": {},
    "description": "A practical functional library for JavaScript programmers.",
    "devDependencies": {
        "acorn": "0.9.x",
        "benchmark": "~1.0.0",
        "browserify": "10.x.x",
        "cli-table": "0.3.x",
        "commander": "2.5.x",
        "dox": "latest",
        "envvar": "1.x.x",
        "escodegen": "1.4.x",
        "eslint": "^2.11.0",
        "handlebars": "3.0.x",
        "istanbul": "^0.4.x",
        "js-yaml": "^3.2.5",
        "jsverify": "^0.7.3",
        "mocha": "2.x.x",
        "q": "^1.1.1",
        "ramda": "0.17.x",
        "rimraf": "~2.3.2",
        "sanctuary": "0.7.x",
        "sinon": "^1.17.4",
        "testem": "0.9.x",
        "uglify-js": "2.4.x",
        "xyz": "1.0.x"
    },
    "directories": {},
    "dist": {
        "shasum": "ccd13fff73497a93974e3e86327bfd87bd6e8e2b",
        "tarball": "https://registry.npmjs.org/ramda/-/ramda-0.23.0.tgz"
    },
    "gitHead": "5dec606e0504af973cd6e0ceec8997b72800eb6b",
    "homepage": "http://ramdajs.com/",
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "aromano",
            "email": "aromano@preemptsecurity.com"
        },
        {
            "name": "buzzdecafe",
            "email": "m_hur@yahoo.com"
        },
        {
            "name": "crosseye",
            "email": "scott@sauyet.com"
        },
        {
            "name": "davidchambers",
            "email": "dc@davidchambers.me"
        },
        {
            "name": "kedashoe",
            "email": "kwallace@gmail.com"
        },
        {
            "name": "rane",
            "email": "raine.virta@gmail.com"
        },
        {
            "name": "scott-christopher",
            "email": "schristopher@konputa.com"
        }
    ],
    "name": "ramda",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/ramda/ramda.git"
    },
    "scripts": {
        "bench": "scripts/benchRunner",
        "bookmarklet": "scripts/bookmarklet",
        "browser_test": "testem ci",
        "build": "make && make dist/ramda.min.js",
        "clean": "rimraf dist/* coverage/*",
        "coverage": "istanbul cover node_modules/.bin/_mocha -- --reporter spec",
        "lint": "eslint scripts/bookmarklet scripts/build src/*.js src/internal/*.js test/*.js test/**/*.js lib/sauce/*.js lib/bench/*.js",
        "postbrowser_test": "npm run posttest",
        "postcoverage": "npm run posttest",
        "posttest": "git checkout -- dist",
        "prebrowser_test": "npm run pretest",
        "precoverage": "npm run pretest",
        "test": "mocha --reporter spec"
    },
    "version": "0.23.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
