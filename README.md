# api documentation for  [json-web-token (v2.1.3)](https://github.com/joaquimserafim/json-web-token)  [![npm package](https://img.shields.io/npm/v/npmdoc-json-web-token.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-json-web-token) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-json-web-token.svg)](https://travis-ci.org/npmdoc/node-npmdoc-json-web-token)
#### JSON Web Token (JWT) is a compact token format intended for space constrained environments such as HTTP Authorization headers and URI query parameters.

[![NPM](https://nodei.co/npm/json-web-token.png?downloads=true)](https://www.npmjs.com/package/json-web-token)

[![apidoc](https://npmdoc.github.io/node-npmdoc-json-web-token/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-json-web-token_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-json-web-token/build/apidoc.html)

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
            "name": "quim",
            "email": "joaquim.serafim@gmail.com"
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
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module json-web-token](#apidoc.module.json-web-token)
1.  [function <span class="apidocSignatureSpan">json-web-token.</span>JWTError (message)](#apidoc.element.json-web-token.JWTError)
1.  [function <span class="apidocSignatureSpan">json-web-token.</span>JWTError.super_ ()](#apidoc.element.json-web-token.JWTError.super_)
1.  [function <span class="apidocSignatureSpan">json-web-token.</span>decode (key, token, cb)](#apidoc.element.json-web-token.decode)
1.  [function <span class="apidocSignatureSpan">json-web-token.</span>encode (key, data, algorithm, cb)](#apidoc.element.json-web-token.encode)
1.  [function <span class="apidocSignatureSpan">json-web-token.</span>getAlgorithms ()](#apidoc.element.json-web-token.getAlgorithms)

#### [module json-web-token.JWTError](#apidoc.module.json-web-token.JWTError)
1.  [function <span class="apidocSignatureSpan">json-web-token.</span>JWTError (message)](#apidoc.element.json-web-token.JWTError.JWTError)
1.  [function <span class="apidocSignatureSpan">json-web-token.JWTError.</span>super_ ()](#apidoc.element.json-web-token.JWTError.super_)

#### [module json-web-token.JWTError.super_](#apidoc.module.json-web-token.JWTError.super_)
1.  [function <span class="apidocSignatureSpan">json-web-token.JWTError.</span>super_ ()](#apidoc.element.json-web-token.JWTError.super_.super_)
1.  [function <span class="apidocSignatureSpan">json-web-token.JWTError.super_.</span>captureStackTrace ()](#apidoc.element.json-web-token.JWTError.super_.captureStackTrace)
1.  number <span class="apidocSignatureSpan">json-web-token.JWTError.super_.</span>stackTraceLimit



# <a name="apidoc.module.json-web-token"></a>[module json-web-token](#apidoc.module.json-web-token)

#### <a name="apidoc.element.json-web-token.JWTError"></a>[function <span class="apidocSignatureSpan">json-web-token.</span>JWTError (message)](#apidoc.element.json-web-token.JWTError)
- description and source-code
```javascript
function JWTError(message) {
  Error.call(this)
  Error.captureStackTrace(this, this.constructor)
  this.name = this.constructor.name
  this.message = message
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.json-web-token.JWTError.super_"></a>[function <span class="apidocSignatureSpan">json-web-token.</span>JWTError.super_ ()](#apidoc.element.json-web-token.JWTError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.json-web-token.decode"></a>[function <span class="apidocSignatureSpan">json-web-token.</span>decode (key, token, cb)](#apidoc.element.json-web-token.decode)
- description and source-code
```javascript
function decode(key, token, cb) {
  if (paramsAreFalsy(key, token)) {
    return prcResult('The key and token are mandatory!', null, cb)
  }

  const parts = token.split('.')

  // check all parts're present
  if (parts.length !== 3) {
    return prcResult(
      'The JWT should consist of three parts!',
      null,
      cb
    )
  }

  // base64 decode and parse JSON
  const header = JSONParse(b64url.decode(parts[0]))
  const payload = JSONParse(b64url.decode(parts[1]))

  // get algorithm hash and type and check if is valid
  const algorithm = algorithms[header.alg]

  if (!algorithm) {
    return prcResult('The algorithm is not supported!', null, cb)
  }

  // verify the signature
  const res = verify(
    algorithm,
    key,
    parts.slice(0, 2).join('.'),
    parts[2]
  )

  return prcResult(!res && 'Invalid key!' || null, payload, header, cb)
}
```
- example usage
```shell
...
jwt.encode(secret, payload, function (err, token) {
if (err) {
  console.error(err.name, err.message);
} else {
  console.log(token);

  // decode
  jwt.decode(secret, token, function (err_, decodedPayload, decodedHeader) {
    if (err) {
      console.error(err.name, err.message);
    } else {
      console.log(decodedPayload, decodedHeader);
    }
  });
}
...
```

#### <a name="apidoc.element.json-web-token.encode"></a>[function <span class="apidocSignatureSpan">json-web-token.</span>encode (key, data, algorithm, cb)](#apidoc.element.json-web-token.encode)
- description and source-code
```javascript
function encode(key, data, algorithm, cb) {
  if (paramIsValid(algorithm, 'function')) {
    cb = algorithm
    algorithm = 'HS256'
  }

  var defaultHeader = {typ: 'JWT', alg: algorithm}

  var payload = isObject(data) && data.payload ?
    data.payload :
    data

  var header = isObject(data) && data.header ?
    extend(data.header, defaultHeader) :
    defaultHeader

  const validationError = encodeValidations(key, payload, algorithm)

  if (validationError) {
    return prcResult(validationError, null, cb)
  }

  const parts = b64url.encode(JSON.stringify(header)) +
    '.' +
    b64url.encode(JSON.stringify(payload))

  return prcResult(
    null,
    parts + '.' + sign(algorithms[algorithm], key, parts),
    cb
  )
}
```
- example usage
```shell
...
"status": "SUCCESS"
  }
};

var secret = 'TOPSECRETTTTT';

// encode
jwt.encode(secret, payload, function (err, token) {
  if (err) {
console.error(err.name, err.message);
  } else {
console.log(token);

// decode
jwt.decode(secret, token, function (err_, decodedPayload, decodedHeader) {
...
```

#### <a name="apidoc.element.json-web-token.getAlgorithms"></a>[function <span class="apidocSignatureSpan">json-web-token.</span>getAlgorithms ()](#apidoc.element.json-web-token.getAlgorithms)
- description and source-code
```javascript
function getAlgorithms() {
  return Object.keys(algorithms)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.json-web-token.JWTError"></a>[module json-web-token.JWTError](#apidoc.module.json-web-token.JWTError)

#### <a name="apidoc.element.json-web-token.JWTError.JWTError"></a>[function <span class="apidocSignatureSpan">json-web-token.</span>JWTError (message)](#apidoc.element.json-web-token.JWTError.JWTError)
- description and source-code
```javascript
function JWTError(message) {
  Error.call(this)
  Error.captureStackTrace(this, this.constructor)
  this.name = this.constructor.name
  this.message = message
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.json-web-token.JWTError.super_"></a>[function <span class="apidocSignatureSpan">json-web-token.JWTError.</span>super_ ()](#apidoc.element.json-web-token.JWTError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.json-web-token.JWTError.super_"></a>[module json-web-token.JWTError.super_](#apidoc.module.json-web-token.JWTError.super_)

#### <a name="apidoc.element.json-web-token.JWTError.super_.super_"></a>[function <span class="apidocSignatureSpan">json-web-token.JWTError.</span>super_ ()](#apidoc.element.json-web-token.JWTError.super_.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.json-web-token.JWTError.super_.captureStackTrace"></a>[function <span class="apidocSignatureSpan">json-web-token.JWTError.super_.</span>captureStackTrace ()](#apidoc.element.json-web-token.JWTError.super_.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
...

//
// JWT token error
//

function JWTError (message) {
  Error.call(this)
  Error.captureStackTrace(this, this.constructor)
  this.name = this.constructor.name
  this.message = message
}

inherits(JWTError, Error)

//
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
