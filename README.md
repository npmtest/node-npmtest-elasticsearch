# npmtest-elasticsearch

#### basic test coverage for  [elasticsearch (v13.0.0)](http://www.elastic.co/guide/en/elasticsearch/client/javascript-api/current/index.html)  [![npm package](https://img.shields.io/npm/v/npmtest-elasticsearch.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-elasticsearch) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-elasticsearch.svg)](https://travis-ci.org/npmtest/node-npmtest-elasticsearch)

#### The official low-level Elasticsearch client for Node.js and the browser.

[![NPM](https://nodei.co/npm/elasticsearch.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/elasticsearch)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-elasticsearch/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-elasticsearch/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-elasticsearch/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-elasticsearch/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-elasticsearch/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-elasticsearch/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-elasticsearch/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-elasticsearch/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-elasticsearch/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-elasticsearch/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-elasticsearch/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-elasticsearch/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-elasticsearch/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-elasticsearch/build/test-report.html](https://npmtest.github.io/node-npmtest-elasticsearch/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-elasticsearch/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-elasticsearch/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-elasticsearch/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-elasticsearch/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-elasticsearch/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-elasticsearch/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-elasticsearch/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-elasticsearch/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Spencer Alger"
    },
    "browser": {
        "./src/lib/connectors/index.js": "./src/lib/connectors/browser_index.js",
        "./src/lib/loggers/index.js": "./src/lib/loggers/browser_index.js",
        "./src/lib/apis/index.js": "./src/lib/apis/browser_index.js",
        "./test/mocks/server.js": "./test/mocks/browser_server.js"
    },
    "bugs": {
        "url": "https://github.com/elastic/elasticsearch-js/issues"
    },
    "config": {
        "blanket": {
            "pattern": "specified in test/unit/coverage.js"
        },
        "default_api_branch": "5.3",
        "supported_es_branches": [
            "5.3",
            "5.2",
            "5.1",
            "5.0",
            "2.4",
            "1.7",
            "0.90"
        ],
        "unstable_es_branches": [
            "5.x",
            "master"
        ]
    },
    "dependencies": {
        "agentkeepalive": "^2.2.0",
        "chalk": "^1.0.0",
        "lodash": "2.4.2",
        "lodash.get": "^4.4.2",
        "lodash.isempty": "^4.4.0",
        "lodash.trimend": "^4.5.1"
    },
    "description": "The official low-level Elasticsearch client for Node.js and the browser.",
    "devDependencies": {
        "@spalger/eslint-config-personal": "^0.4.0",
        "async": "~0.8.0",
        "babel-eslint": "^6.0.4",
        "blanket": "^1.2.3",
        "bluebird": "^2.9.14",
        "eslint": "^2.9.0",
        "eslint-config-airbnb": "^8.0.0",
        "eslint-plugin-import": "^1.6.1",
        "eslint-plugin-jsx-a11y": "^1.0.4",
        "eslint-plugin-react": "^5.0.1",
        "expect.js": "^0.3.1",
        "express": "~3.4.7",
        "find-root": "~0.1.1",
        "glob": "~3.2.7",
        "grunt": "^1.0.1",
        "grunt-cli": "^1.2.0",
        "grunt-contrib-clean": "^1.0.0",
        "grunt-contrib-compress": "^1.2.0",
        "grunt-contrib-concat": "^1.0.1",
        "grunt-contrib-copy": "^1.0.0",
        "grunt-contrib-uglify": "^1.0.1",
        "grunt-contrib-watch": "^1.0.0",
        "grunt-esvm": "^3.2.8",
        "grunt-mocha-cov": "^0.4.0",
        "grunt-open": "~0.2.2",
        "grunt-prompt": "^1.3.3",
        "grunt-run": "^0.6.0",
        "grunt-s3": "~0.2.0-alpha.3",
        "grunt-saucelabs": "^8.6.2",
        "grunt-webpack": "^1.0.11",
        "jquery": "^2.2.3",
        "js-yaml": "^3.6.0",
        "load-grunt-config": "^0.19.2",
        "load-grunt-tasks": "^3.5.0",
        "mocha": "^2.2.5",
        "mocha-lcov-reporter": "0.0.1",
        "mocha-screencast-reporter": "~0.1.4",
        "moment": "^2.13.0",
        "nock": "~0.28.3",
        "null-loader": "^0.1.1",
        "open": "0.0.5",
        "optimist": "~0.6.0",
        "semver": "^4.3.6",
        "sinon": "^1.17.4",
        "split": "~0.3.2",
        "through2": "~0.6.3",
        "through2-map": "~1.4.0",
        "webpack": "^1.13.0",
        "webpack-dev-server": "^1.14.1",
        "xmlbuilder": "~0.4.3"
    },
    "directories": {},
    "dist": {
        "shasum": "7f95bdbff5cad637a53be613ddb9adf3770cef58",
        "tarball": "https://registry.npmjs.org/elasticsearch/-/elasticsearch-13.0.0.tgz"
    },
    "engines": {
        "node": ">=0.8"
    },
    "gitHead": "5e9afef1ad964ea7c64ab9de8a33937cb359cf09",
    "homepage": "http://www.elastic.co/guide/en/elasticsearch/client/javascript-api/current/index.html",
    "keywords": [
        "elasticsearch",
        "mapping",
        "REST"
    ],
    "license": "Apache-2.0",
    "main": "src/elasticsearch.js",
    "maintainers": [
        {
            "name": "lukasolson"
        },
        {
            "name": "spalger"
        },
        {
            "name": "tylersmalley"
        }
    ],
    "name": "elasticsearch",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/elastic/elasticsearch-js.git"
    },
    "scripts": {
        "eslint": "eslint src scripts test grunt Gruntfile.js",
        "generate": "node scripts/generate",
        "grunt": "grunt",
        "test": "grunt test"
    },
    "version": "13.0.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
