# npmtest-snapchat

#### basic test coverage for  snapchat (v2.0.2)  [![npm package](https://img.shields.io/npm/v/npmtest-snapchat.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-snapchat) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-snapchat.svg)](https://travis-ci.org/npmtest/node-npmtest-snapchat)

#### Nodejs client for the unofficial Snapchat API

[![NPM](https://nodei.co/npm/snapchat.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/snapchat)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-snapchat/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-snapchat/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-snapchat/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-snapchat/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-snapchat/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-snapchat/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-snapchat/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-snapchat/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-snapchat/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-snapchat/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-snapchat/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-snapchat/build/test-report.html](https://npmtest.github.io/node-npmtest-snapchat/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-snapchat/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-snapchat/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-snapchat/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-snapchat/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-snapchat/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-snapchat/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-snapchat/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-snapchat/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "snapchat",
    "description": "Nodejs client for the unofficial Snapchat API",
    "version": "2.0.2",
    "author": {
        "name": "Travis Fischer",
        "url": "https://makesnaps.com"
    },
    "bugs": {
        "url": "https://github.com/fisch0920/snapchat/issues"
    },
    "dependencies": {
        "async": "^1.4.2",
        "bignum": "^0.11.0",
        "bluebird": "^2.9.34",
        "debug": "^2.1.0",
        "enum": "^2.1.0",
        "file-type": "^2.10.2",
        "iconv-lite": "^0.4.11",
        "inherits": "^2.0.1",
        "jszip": "^2.5.0",
        "node-rsa": "^0.2.25",
        "node-uuid": "^1.4.3",
        "phone": "^1.0.4",
        "request": "^2.61.0",
        "url-join": "0.0.1",
        "ursa": "^0.8.5",
        "xtend": "^4.0.0"
    },
    "devDependencies": {
        "browserify": "^10.0.0",
        "dotenv": "^1.2.0",
        "gulp": "^3.9.0",
        "gulp-gh-pages": "^0.5.2",
        "gulp-npm-run": "0.0.1",
        "ink-docstrap": "git://github.com/fisch0920/docstrap",
        "jsdoc": "^3.3.2",
        "standard": "^4.0.1",
        "tape": "^4.0.0",
        "uglify-js": "^2.4.15"
    },
    "keywords": [
        "snapchat",
        "api",
        "unofficial",
        "snap",
        "chat",
        "sc",
        "image",
        "video",
        "REST",
        "client"
    ],
    "license": "MIT",
    "main": "index.js",
    "repository": {
        "type": "git",
        "url": "git://github.com/fisch0920/snapchat.git"
    },
    "scripts": {
        "build": "browserify -s Snapchat -e ./ | uglifyjs -m > snapchat.min.js",
        "build-debug": "browserify -s Snapchat -e ./ > snapchat.debug.js",
        "docs": "node ./node_modules/jsdoc/jsdoc.js -c .jsdoc.json -R README.md",
        "size": "npm run build && cat snapchat.min.js | gzip | wc -c",
        "test": "standard && tape test/*.js",
        "test-node": "tape test/*.js"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
