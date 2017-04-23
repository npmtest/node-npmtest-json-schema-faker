# npmtest-json-schema-faker

#### basic test coverage for  [json-schema-faker (v0.5.0-rc1)](http://json-schema-faker.js.org)  [![npm package](https://img.shields.io/npm/v/npmtest-json-schema-faker.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-json-schema-faker) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-json-schema-faker.svg)](https://travis-ci.org/npmtest/node-npmtest-json-schema-faker)

#### JSON-Schema + fake data generators

[![NPM](https://nodei.co/npm/json-schema-faker.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/json-schema-faker)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-json-schema-faker/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-json-schema-faker/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-json-schema-faker/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-json-schema-faker/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-json-schema-faker/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-json-schema-faker/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-json-schema-faker/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-json-schema-faker/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-json-schema-faker/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-json-schema-faker/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-json-schema-faker/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-json-schema-faker/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-json-schema-faker/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-json-schema-faker/build/test-report.html](https://npmtest.github.io/node-npmtest-json-schema-faker/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-json-schema-faker/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-json-schema-faker/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-json-schema-faker/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-json-schema-faker/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-json-schema-faker/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-json-schema-faker/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-json-schema-faker/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-json-schema-faker/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/json-schema-faker/json-schema-faker/issues"
    },
    "contributors": [
        {
            "name": "Alvaro Cabrera",
            "url": "https://soypache.co"
        },
        {
            "name": "Tomasz Ducin",
            "url": "http://ducin.it"
        }
    ],
    "dependencies": {
        "json-schema-ref-parser": "3.1.2",
        "randexp": "0.4.3",
        "tslib": "1.4.0"
    },
    "description": "JSON-Schema + fake data generators",
    "devDependencies": {
        "casual-cjs": "1.5.10",
        "chance": "1.0.4",
        "clone": "2.1.0",
        "codecov": "1.0.1",
        "faker": "4.1.0",
        "fs-extra": "1.0.0",
        "glob": "7.1.1",
        "istanbul": "0.4.5",
        "jasmine-node": "2.0.0-beta4",
        "jayschema": "0.3.1",
        "lodash.template": "4.4.0",
        "rollup": "0.38.0",
        "rollup-plugin-commonjs": "^7.0.0",
        "rollup-plugin-node-resolve": "^2.0.0",
        "semver": "5.3.0",
        "tarima-cli": "github:gextech/tarima-cli",
        "ts-node": "2.1.0",
        "tslint": "4.0.2",
        "tv4": "1.2.7",
        "typedoc": "0.5.1",
        "typescript": "2.1.1",
        "uglify-js": "2.7.4",
        "z-schema": "3.18.1"
    },
    "directories": {},
    "dist": {
        "shasum": "6242d6c4fea81543f2364466b84de30648a813c0",
        "tarball": "https://registry.npmjs.org/json-schema-faker/-/json-schema-faker-0.5.0-rc1.tgz"
    },
    "gitHead": "20d7f2a4ba74f6c02c7cc5d5b037414b87f71a69",
    "homepage": "http://json-schema-faker.js.org",
    "keywords": [
        "json",
        "jsonschema",
        "fake",
        "mocks"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "pateketrueke"
        },
        {
            "name": "ducin"
        }
    ],
    "name": "json-schema-faker",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/json-schema-faker/json-schema-faker.git"
    },
    "scripts": {
        "build": "tarima -qf",
        "build:dist": "node build/dist.js",
        "cover:schema": "istanbul cover --root lib --x '**/spec/**' -- jasmine-node --coffee spec/schema",
        "cover:unit": "istanbul cover --root lib --x '**/spec/**' -- jasmine-node --coffee spec/unit",
        "cover:up": "codecov --file=coverage/lcov.info --disable=gcov -e TRAVIS_NODE_VERSION",
        "dev": "jasmine-node spec/schema --coffee --verbose --autoTest --watchFolders lib",
        "dev:unit": "jasmine-node spec/unit --coffee --verbose --autoTest --watchFolders lib",
        "dist": "yarn build && yarn build:dist",
        "graphviz": "madge lib --dot > structure.gv",
        "test": "yarn test:lint && yarn build && yarn test:unit && yarn test:schema",
        "test:lint": "tslint ts/**/*.ts",
        "test:schema": "jasmine-node spec/schema --coffee --noStackTrace --captureExceptions",
        "test:unit": "jasmine-node spec/unit --noStackTrace --captureExceptions",
        "typedoc": "typedoc --out docs/html ts/ --module commonjs"
    },
    "tarima": {
        "src": "ts/**",
        "dest": "lib",
        "bundle": true,
        "ignore": [
            "**/*.d.ts"
        ],
        "filter": [
            "!*/*/**"
        ],
        "rename": [
            "ts/**:{filepath/1}/{filename}.{extname}"
        ],
        "bundleOptions": {
            "rollup": {
                "bundle": "JSONSchemaFaker",
                "format": "cjs",
                "interop": false
            }
        }
    },
    "version": "0.5.0-rc1",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
