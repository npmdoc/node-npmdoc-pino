# npmdoc-pino

#### api documentation for  [pino (v4.3.0)](https://github.com/pinojs/pino#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-pino.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-pino) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-pino.svg)](https://travis-ci.org/npmdoc/node-npmdoc-pino)

#### super fast, all natural json logger

[![NPM](https://nodei.co/npm/pino.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/pino)

- [https://npmdoc.github.io/node-npmdoc-pino/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-pino/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-pino/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-pino/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-pino/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-pino/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Matteo Collina"
    },
    "bin": {
        "pino": "./bin.js"
    },
    "browser": "./browser.js",
    "bugs": {
        "url": "https://github.com/pinojs/pino/issues"
    },
    "contributors": [
        {
            "name": "David Mark Clements"
        },
        {
            "name": "James Sumners"
        },
        {
            "name": "Thomas Watson Steen",
            "url": "https://twitter.com/wa7son"
        }
    ],
    "dependencies": {
        "chalk": "^1.1.1",
        "fast-json-parse": "^1.0.0",
        "fast-safe-stringify": "^1.1.11",
        "flatstr": "^1.0.4",
        "pump": "^1.0.2",
        "quick-format-unescaped": "^1.1.1",
        "split2": "^2.0.1"
    },
    "description": "super fast, all natural json logger",
    "devDependencies": {
        "benchmark": "^2.1.2",
        "bole": "^3.0.2",
        "bunyan": "^1.8.5",
        "debug": "^2.5.1",
        "fastbench": "^1.0.0",
        "flush-write-stream": "^1.0.2",
        "fresh-require": "^1.0.3",
        "log": "^1.4.0",
        "loglevel": "^1.4.0",
        "pre-commit": "^1.2.2",
        "snazzy": "^6.0.0",
        "standard": "^10.0.0",
        "steed": "^1.1.3",
        "tap": "^10.0.0",
        "tape": "^4.6.2",
        "through2": "^2.0.1",
        "winston": "^2.3.0",
        "zuul": "^3.11.1"
    },
    "directories": {},
    "dist": {
        "shasum": "67c5ef9ef9d39db1d28aa46c535262153574205a",
        "tarball": "https://registry.npmjs.org/pino/-/pino-4.3.0.tgz"
    },
    "files": [
        "pino.js",
        "bin.js",
        "browser.js",
        "pretty.js",
        "usage.txt",
        "test",
        "docs",
        "example.js",
        "lib"
    ],
    "gitHead": "74bc0fd8af2ee10d398ab7a6d9a0207ee138405c",
    "homepage": "https://github.com/pinojs/pino#readme",
    "keywords": [
        "fast",
        "logger",
        "stream",
        "json"
    ],
    "license": "MIT",
    "main": "pino.js",
    "maintainers": [
        {
            "name": "davidmarkclements"
        },
        {
            "name": "jsumners"
        },
        {
            "name": "matteo.collina"
        },
        {
            "name": "watson"
        }
    ],
    "name": "pino",
    "optionalDependencies": {},
    "precommit": "test",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/pinojs/pino.git"
    },
    "scripts": {
        "bench-all": "node benchmarks/runbench all",
        "bench-basic": "node benchmarks/runbench basic",
        "bench-child": "node benchmarks/runbench child",
        "bench-conception": "node benchmarks/runbench conception",
        "bench-deepobject": "node benchmarks/runbench deepobject",
        "bench-grandchild": "node benchmarks/runbench grandchild",
        "bench-longstring": "node benchmarks/runbench longstring",
        "bench-multiarg": "node benchmarks/runbench multiarg",
        "bench-object": "node benchmarks/runbench object",
        "browser-test": "zuul tape test/browser.test.js --local",
        "ci": "standard | snazzy && tap --cov test/*test.js",
        "test": "standard | snazzy && tap --no-cov test/*test.js"
    },
    "version": "4.3.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
