# npmdoc-json-web-token

#### api documentation for  [json-web-token (v2.1.3)](https://github.com/joaquimserafim/json-web-token)  [![npm package](https://img.shields.io/npm/v/npmdoc-json-web-token.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-json-web-token) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-json-web-token.svg)](https://travis-ci.org/npmdoc/node-npmdoc-json-web-token)

#### JSON Web Token (JWT) is a compact token format intended for space constrained environments such as HTTP Authorization headers and URI query parameters.

[![NPM](https://nodei.co/npm/json-web-token.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/json-web-token)

- [https://npmdoc.github.io/node-npmdoc-json-web-token/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-json-web-token/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-json-web-token/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-json-web-token/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-json-web-token/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-json-web-token/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "@joaquimserafim"
    },
    "bugs": {
        "url": "https://github.com/joaquimserafim/json-web-token/issues"
    },
    "dependencies": {
        "base64-url": "^1.2.2",
        "is.object": "^1.0.0",
        "json-parse-safe": "^1.0.3",
        "xtend": "^4.0.1"
    },
    "description": "JSON Web Token (JWT) is a compact token format intended for space constrained environments such as HTTP Authorization headers and URI query parameters.",
    "devDependencies": {
        "istanbul": "0.4.3",
        "jscs": "^2.11.0",
        "jshint": "^2.9.2",
        "nsp": "^2.4.0",
        "plato": "^1.5.0",
        "pre-commit": "^1.1.3",
        "tap-spec": "^4.1.1",
        "tape": "^4.5.1"
    },
    "directories": {},
    "dist": {
        "shasum": "ec2e3bdf7481db980cbfc06d7ff03de211cd7877",
        "tarball": "https://registry.npmjs.org/json-web-token/-/json-web-token-2.1.3.tgz"
    },
    "engine": {
        "node": ">=4"
    },
    "files": [
        "LICENSE",
        "README.md",
        "index.js"
    ],
    "gitHead": "412c2c8ebd844b0187d81d14f70e1268d19d9476",
    "homepage": "https://github.com/joaquimserafim/json-web-token",
    "keywords": [
        "jwt",
        "json-web-token",
        "web",
        "http",
        "tokens",
        "authorization"
    ],
    "license": "ISC",
    "main": "index.js",
    "maintainers": [
        {
            "name": "quim"
        }
    ],
    "name": "json-web-token",
    "optionalDependencies": {},
    "pre-commit": [
        "lint",
        "style",
        "coverage",
        "security"
    ],
    "repository": {
        "type": "git",
        "url": "git://github.com/joaquimserafim/json-web-token.git"
    },
    "scripts": {
        "bench": "echo 'installing dependencies first ...' && sleep 1 && npm i --save-dev benchmark microtime && echo '' && node bench && npm uninstall --save-dev benchmark microtime",
        "complexity": "plato -r -t 'jenkins-client code report' -l .jshintrc -x 'node_modules|reports|test|bench' -d reports/plato .",
        "complexity:open": "open reports/plato/index.html",
        "coverage": "istanbul cover tape test/test.js && istanbul check-coverage",
        "coverage:open": "open reports/coverage/index.html",
        "lint": "jshint -c .jshintrc index.js test/test.js",
        "security": "nsp check",
        "style": "jscs -p google index.js test/test.js",
        "test": "tape test/test.js | tap-spec"
    },
    "version": "2.1.3"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
