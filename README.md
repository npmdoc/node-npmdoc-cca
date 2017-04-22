# npmdoc-cca

#### api documentation for  [cca (v0.8.1)](https://github.com/MobileChromeApps/mobile-chrome-apps#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-cca.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-cca) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-cca.svg)](https://travis-ci.org/npmdoc/node-npmdoc-cca)

#### Run Chrome Apps on mobile using Apache Cordova

[![NPM](https://nodei.co/npm/cca.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/cca)

- [https://npmdoc.github.io/node-npmdoc-cca/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-cca/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-cca/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-cca/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-cca/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-cca/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "cca",
    "author": {
        "name": "The Chrome Team"
    },
    "version": "0.8.1",
    "description": "Run Chrome Apps on mobile using Apache Cordova",
    "preferGlobal": "true",
    "keywords": [
        "cordova",
        "chrome",
        "mobile",
        "apps"
    ],
    "bin": {
        "cca": "src/cca.js"
    },
    "main": "src/cca.js",
    "man": [
        "./docs/man/cca.7"
    ],
    "license": "Apache-2.0",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/MobileChromeApps/mobile-chrome-apps.git"
    },
    "dependencies": {
        "cca-manifest-logic": "^1.1.5",
        "chrome-app-developer-tool-client": "^0.0.5",
        "cordova": "^5.4.0",
        "crypto-js": "^3.1.4",
        "debounce": "^1.0.0",
        "elementtree": "0.1.6",
        "gaze": "^0.5.1",
        "node-uuid": "^1.4.1",
        "node.extend": "",
        "optimist": "~0.6.1",
        "q": "~1",
        "semver": "^4.1.0",
        "shelljs": "^0.4.0",
        "underscore": "^1.7.0",
        "update-notifier": "^0.5.0",
        "xmldom": "^0.1.19"
    },
    "files": [
        "README.md",
        "RELEASENOTES.md",
        "cordova",
        "docs",
        "src",
        "templates"
    ],
    "devDependencies": {
        "chai": "^1.9.1",
        "gulp": "^3.7.0",
        "gulp-jshint": "^1.6.1",
        "gulp-mocha": "^1.1.1",
        "gulp-util": "^3.0.1",
        "walk": "^2.3.3"
    },
    "scripts": {
        "test": "gulp test"
    },
    "bugs": {
        "url": "https://github.com/MobileChromeApps/mobile-chrome-apps/issues"
    },
    "homepage": "https://github.com/MobileChromeApps/mobile-chrome-apps#readme",
    "maintainers": [
        {
            "name": "agrieve"
        },
        {
            "name": "mmocny"
        },
        {
            "name": "shepheb"
        },
        {
            "name": "maxw"
        },
        {
            "name": "clelland"
        },
        {
            "name": "kamrik"
        },
        {
            "name": "drkemp"
        }
    ],
    "dist": {
        "shasum": "9bc7a526b5e8f638a46ff994f8258731970a2caa",
        "tarball": "https://registry.npmjs.org/cca/-/cca-0.8.1.tgz"
    },
    "directories": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
