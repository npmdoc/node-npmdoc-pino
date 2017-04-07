# api documentation for  [pino (v4.2.4)](https://github.com/pinojs/pino#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-pino.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-pino) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-pino.svg)](https://travis-ci.org/npmdoc/node-npmdoc-pino)
#### super fast, all natural json logger

[![NPM](https://nodei.co/npm/pino.png?downloads=true)](https://www.npmjs.com/package/pino)

[![apidoc](https://npmdoc.github.io/node-npmdoc-pino/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-pino_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-pino/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-pino/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-pino/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Matteo Collina",
        "email": "hello@matteocollina.com"
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
            "name": "David Mark Clements",
            "email": "huperekchuno@googlemail.com"
        },
        {
            "name": "James Sumners",
            "email": "james.sumners@gmail.com"
        },
        {
            "name": "Thomas Watson Steen",
            "email": "w@tson.dk",
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
        "standard": "^9.0.0",
        "steed": "^1.1.3",
        "tap": "^10.0.0",
        "tape": "^4.6.2",
        "through2": "^2.0.1",
        "winston": "^2.3.0",
        "zuul": "^3.11.1"
    },
    "directories": {},
    "dist": {
        "shasum": "e893cc31446402574aa976816e5c373e869106fa",
        "tarball": "https://registry.npmjs.org/pino/-/pino-4.2.4.tgz"
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
    "gitHead": "e5e455049e24da61f7f168e2b6e5392524535c8f",
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
            "name": "davidmarkclements",
            "email": "huperekchuno@googlemail.com"
        },
        {
            "name": "jsumners",
            "email": "james.sumners@gmail.com"
        },
        {
            "name": "matteo.collina",
            "email": "hello@matteocollina.com"
        },
        {
            "name": "watson",
            "email": "w@tson.dk"
        }
    ],
    "name": "pino",
    "optionalDependencies": {},
    "precommit": "test",
    "readme": "ERROR: No README data found!",
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
    "version": "4.2.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module pino](#apidoc.module.pino)
1.  [function <span class="apidocSignatureSpan">pino.</span>pretty (opts)](#apidoc.element.pino.pretty)
1.  number <span class="apidocSignatureSpan">pino.</span>LOG_VERSION
1.  object <span class="apidocSignatureSpan">pino.</span>levels
1.  object <span class="apidocSignatureSpan">pino.</span>serializers
1.  object <span class="apidocSignatureSpan">pino.</span>stdSerializers
1.  object <span class="apidocSignatureSpan">pino.</span>time
1.  object <span class="apidocSignatureSpan">pino.</span>tools

#### [module pino.levels](#apidoc.module.pino.levels)
1.  [function <span class="apidocSignatureSpan">pino.levels.</span>isStandardLevel (level)](#apidoc.element.pino.levels.isStandardLevel)
1.  [function <span class="apidocSignatureSpan">pino.levels.</span>isStandardLevelVal (val)](#apidoc.element.pino.levels.isStandardLevelVal)
1.  object <span class="apidocSignatureSpan">pino.</span>levels
1.  object <span class="apidocSignatureSpan">pino.levels.</span>lscache
1.  object <span class="apidocSignatureSpan">pino.levels.</span>nums

#### [module pino.serializers](#apidoc.module.pino.serializers)
1.  [function <span class="apidocSignatureSpan">pino.serializers.</span>asErrValue (err)](#apidoc.element.pino.serializers.asErrValue)
1.  [function <span class="apidocSignatureSpan">pino.serializers.</span>asReqValue (req)](#apidoc.element.pino.serializers.asReqValue)
1.  [function <span class="apidocSignatureSpan">pino.serializers.</span>asResValue (res)](#apidoc.element.pino.serializers.asResValue)
1.  [function <span class="apidocSignatureSpan">pino.serializers.</span>mapHttpRequest (req)](#apidoc.element.pino.serializers.mapHttpRequest)
1.  [function <span class="apidocSignatureSpan">pino.serializers.</span>mapHttpResponse (res)](#apidoc.element.pino.serializers.mapHttpResponse)

#### [module pino.stdSerializers](#apidoc.module.pino.stdSerializers)
1.  [function <span class="apidocSignatureSpan">pino.stdSerializers.</span>err (err)](#apidoc.element.pino.stdSerializers.err)
1.  [function <span class="apidocSignatureSpan">pino.stdSerializers.</span>req (req)](#apidoc.element.pino.stdSerializers.req)
1.  [function <span class="apidocSignatureSpan">pino.stdSerializers.</span>res (res)](#apidoc.element.pino.stdSerializers.res)

#### [module pino.time](#apidoc.module.pino.time)
1.  [function <span class="apidocSignatureSpan">pino.time.</span>getNoTime ()](#apidoc.element.pino.time.getNoTime)
1.  [function <span class="apidocSignatureSpan">pino.time.</span>getSlowTime ()](#apidoc.element.pino.time.getSlowTime)
1.  [function <span class="apidocSignatureSpan">pino.time.</span>getTime ()](#apidoc.element.pino.time.getTime)

#### [module pino.tools](#apidoc.module.pino.tools)
1.  [function <span class="apidocSignatureSpan">pino.tools.</span>applyOptions (opts)](#apidoc.element.pino.tools.applyOptions)
1.  [function <span class="apidocSignatureSpan">pino.tools.</span>copy (a, b)](#apidoc.element.pino.tools.copy)
1.  [function <span class="apidocSignatureSpan">pino.tools.</span>defineLevelsProperty (onObject)](#apidoc.element.pino.tools.defineLevelsProperty)
1.  [function <span class="apidocSignatureSpan">pino.tools.</span>genLog (z)](#apidoc.element.pino.tools.genLog)
1.  [function <span class="apidocSignatureSpan">pino.tools.</span>noop ()](#apidoc.element.pino.tools.noop)
1.  [function <span class="apidocSignatureSpan">pino.tools.</span>streamIsBlockable (s)](#apidoc.element.pino.tools.streamIsBlockable)



# <a name="apidoc.module.pino"></a>[module pino](#apidoc.module.pino)

#### <a name="apidoc.element.pino.pretty"></a>[function <span class="apidocSignatureSpan">pino.</span>pretty (opts)](#apidoc.element.pino.pretty)
- description and source-code
```javascript
function pretty(opts) {
  var timeTransOnly = opts && opts.timeTransOnly
  var formatter = opts && opts.formatter
  var levelFirst = opts && opts.levelFirst

  var stream = split(mapLine)
  var ctx
  var levelColors

  var pipe = stream.pipe

  stream.pipe = function (dest, opts) {
    ctx = new chalk.constructor({
      enabled: !!(chalk.supportsColor && dest.isTTY)
    })

    levelColors = {
      default: ctx.white,
      60: ctx.bgRed,
      50: ctx.red,
      40: ctx.yellow,
      30: ctx.green,
      20: ctx.blue,
      10: ctx.grey
    }

    pipe.call(stream, dest, opts)
  }

  return stream

  function mapLine (line) {
    var parsed = new Parse(line)
    var value = parsed.value

    if (parsed.err || !isPinoLine(value)) {
      // pass through
      return line + '\n'
    }

    if (formatter) {
      return opts.formatter(parsed.value) + '\n'
    }

    if (timeTransOnly) {
      value.time = asISODate(value.time)
      return JSON.stringify(value) + '\n'
    }

    line = (levelFirst)
        ? asColoredLevel(value) + ' [' + asISODate(value.time) + ']'
        : '[' + asISODate(value.time) + '] ' + asColoredLevel(value)

    line += ' ('
    if (value.name) {
      line += value.name + '/'
    }
    line += value.pid + ' on ' + value.hostname + ')'
    line += ': '
    if (value.msg) {
      line += ctx.cyan(value.msg)
    }
    line += '\n'
    if (value.type === 'Error') {
      line += '    ' + withSpaces(value.stack) + '\n'
    } else {
      line += filter(value)
    }
    return line
  }

  function asISODate (time) {
    return new Date(time).toISOString()
  }

  function asColoredLevel (value) {
    if (levelColors.hasOwnProperty(value.level)) {
      return levelColors[value.level](levels[value.level])
    } else {
      return levelColors.default(levels.default)
    }
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.pino.levels"></a>[module pino.levels](#apidoc.module.pino.levels)

#### <a name="apidoc.element.pino.levels.isStandardLevel"></a>[function <span class="apidocSignatureSpan">pino.levels.</span>isStandardLevel (level)](#apidoc.element.pino.levels.isStandardLevel)
- description and source-code
```javascript
isStandardLevel = function (level) {
  if (Infinity === level) {
    return true
  }
  return keys.indexOf(level) > -1
}
```
- example usage
```shell
...
  this._levelVal = num

  for (var key in this.levels.values) {
    if (num > this.levels.values[key]) {
      this[key] = tools.noop
      continue
    }
    this[key] = levels.isStandardLevel(key) ? pinoPrototype[key] : tools.genLog(this.levels.values[key])
  }
}
Object.defineProperty(pinoPrototype, 'levelVal', {
  get: getLevelVal,
  set: setLevelVal
})
...
```

#### <a name="apidoc.element.pino.levels.isStandardLevelVal"></a>[function <span class="apidocSignatureSpan">pino.levels.</span>isStandardLevelVal (val)](#apidoc.element.pino.levels.isStandardLevelVal)
- description and source-code
```javascript
isStandardLevelVal = function (val) {
  if (!isFinite(val)) {
    return true
  }
  return keys.indexOf(val + '') > -1
}
```
- example usage
```shell
...
    data += '"' + key + '":' + this.stringify(value) + ','
  }
}
data = this.chindings + data.substr(0, data.length - 1)

var opts = {
  level: bindings.level || this.level,
  levelVal: levels.isStandardLevelVal(this.levelVal) ? undefined : this.levelVal,
  serializers: bindings.hasOwnProperty('serializers') ? Object.assign({}, this.serializers, bindings.serializers) : this.serializers
,
  stringify: this.stringify,
  end: this.end,
  name: this.name,
  timestamp: this.timestamp,
  slowtime: this.slowtime,
  chindings: data,
...
```



# <a name="apidoc.module.pino.serializers"></a>[module pino.serializers](#apidoc.module.pino.serializers)

#### <a name="apidoc.element.pino.serializers.asErrValue"></a>[function <span class="apidocSignatureSpan">pino.serializers.</span>asErrValue (err)](#apidoc.element.pino.serializers.asErrValue)
- description and source-code
```javascript
function asErrValue(err) {
  var obj = {
    type: err.constructor.name,
    message: err.message,
    stack: err.stack
  }
  for (var key in err) {
    if (obj[key] === undefined) {
      obj[key] = err[key]
    }
  }
  return obj
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pino.serializers.asReqValue"></a>[function <span class="apidocSignatureSpan">pino.serializers.</span>asReqValue (req)](#apidoc.element.pino.serializers.asReqValue)
- description and source-code
```javascript
function asReqValue(req) {
  return {
    method: req.method,
    url: req.url,
    headers: req.headers,
    remoteAddress: req.connection.remoteAddress,
    remotePort: req.connection.remotePort
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pino.serializers.asResValue"></a>[function <span class="apidocSignatureSpan">pino.serializers.</span>asResValue (res)](#apidoc.element.pino.serializers.asResValue)
- description and source-code
```javascript
function asResValue(res) {
  return {
    statusCode: res.statusCode,
    header: res._header
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pino.serializers.mapHttpRequest"></a>[function <span class="apidocSignatureSpan">pino.serializers.</span>mapHttpRequest (req)](#apidoc.element.pino.serializers.mapHttpRequest)
- description and source-code
```javascript
function mapHttpRequest(req) {
  return {
    req: asReqValue(req)
  }
}
```
- example usage
```shell
...
var p
if (typeof a === 'object' && a !== null) {
  m = a
  n = [b, c, d, e, f, g, h, i, j, k]
  l = 1

  if (m.method && m.headers && m.socket) {
    m = serializers.mapHttpRequest(m)
  } else if (typeof m.setHeader === 'function') {
    m = serializers.mapHttpResponse(m)
  }
} else {
  n = [a, b, c, d, e, f, g, h, i, j, k]
}
p = n.length = arguments.length - l
...
```

#### <a name="apidoc.element.pino.serializers.mapHttpResponse"></a>[function <span class="apidocSignatureSpan">pino.serializers.</span>mapHttpResponse (res)](#apidoc.element.pino.serializers.mapHttpResponse)
- description and source-code
```javascript
function mapHttpResponse(res) {
  return {
    res: asResValue(res)
  }
}
```
- example usage
```shell
...
  m = a
  n = [b, c, d, e, f, g, h, i, j, k]
  l = 1

  if (m.method && m.headers && m.socket) {
    m = serializers.mapHttpRequest(m)
  } else if (typeof m.setHeader === 'function') {
    m = serializers.mapHttpResponse(m)
  }
} else {
  n = [a, b, c, d, e, f, g, h, i, j, k]
}
p = n.length = arguments.length - l
if (p > 1) {
  l = typeof a === 'string' ? countInterp(a, '%j') : 0
...
```



# <a name="apidoc.module.pino.stdSerializers"></a>[module pino.stdSerializers](#apidoc.module.pino.stdSerializers)

#### <a name="apidoc.element.pino.stdSerializers.err"></a>[function <span class="apidocSignatureSpan">pino.stdSerializers.</span>err (err)](#apidoc.element.pino.stdSerializers.err)
- description and source-code
```javascript
function asErrValue(err) {
  var obj = {
    type: err.constructor.name,
    message: err.message,
    stack: err.stack
  }
  for (var key in err) {
    if (obj[key] === undefined) {
      obj[key] = err[key]
    }
  }
  return obj
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pino.stdSerializers.req"></a>[function <span class="apidocSignatureSpan">pino.stdSerializers.</span>req (req)](#apidoc.element.pino.stdSerializers.req)
- description and source-code
```javascript
function asReqValue(req) {
  return {
    method: req.method,
    url: req.url,
    headers: req.headers,
    remoteAddress: req.connection.remoteAddress,
    remotePort: req.connection.remotePort
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pino.stdSerializers.res"></a>[function <span class="apidocSignatureSpan">pino.stdSerializers.</span>res (res)](#apidoc.element.pino.stdSerializers.res)
- description and source-code
```javascript
function asResValue(res) {
  return {
    statusCode: res.statusCode,
    header: res._header
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.pino.time"></a>[module pino.time](#apidoc.module.pino.time)

#### <a name="apidoc.element.pino.time.getNoTime"></a>[function <span class="apidocSignatureSpan">pino.time.</span>getNoTime ()](#apidoc.element.pino.time.getNoTime)
- description and source-code
```javascript
function getNoTime() {
  return ''
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pino.time.getSlowTime"></a>[function <span class="apidocSignatureSpan">pino.time.</span>getSlowTime ()](#apidoc.element.pino.time.getSlowTime)
- description and source-code
```javascript
function getSlowTime() {
  return ',"time":"' + (new Date()).toISOString() + '"'
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pino.time.getTime"></a>[function <span class="apidocSignatureSpan">pino.time.</span>getTime ()](#apidoc.element.pino.time.getTime)
- description and source-code
```javascript
function getTime() {
  return ',"time":' + Date.now()
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.pino.tools"></a>[module pino.tools](#apidoc.module.pino.tools)

#### <a name="apidoc.element.pino.tools.applyOptions"></a>[function <span class="apidocSignatureSpan">pino.tools.</span>applyOptions (opts)](#apidoc.element.pino.tools.applyOptions)
- description and source-code
```javascript
function applyOptions(opts) {
  this.serializers = opts.serializers
  this.stringify = opts.stringify
  this.end = opts.end
  this.name = opts.name
  this.timestamp = opts.timestamp
  this.slowtime = opts.slowtime
  this.chindings = opts.chindings
  this.cache = opts.cache
  this.formatOpts = opts.formatOpts
  this.onTerminated = opts.onTerminated

  if (opts.level && opts.levelVal) {
    var levelIsStandard = levels.isStandardLevel(opts.level)
    var valIsStandard = levels.isStandardLevelVal(opts.levelVal)
    if (valIsStandard) throw Error('level value is already used: ' + opts.levelVal)
    if (levelIsStandard === false && valIsStandard === false) this.addLevel(opts.level, opts.levelVal)
  }
  this._setLevel(opts.level)
  this._baseLog = flatstr(baseLog +
    (this.name === undefined ? '' : '"name":' + this.stringify(this.name) + ','))

  if (opts.timestamp === false) {
    this.time = time.getNoTime
  } else if (opts.slowtime) {
    this.time = time.getSlowTime
  } else {
    this.time = time.getTime
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pino.tools.copy"></a>[function <span class="apidocSignatureSpan">pino.tools.</span>copy (a, b)](#apidoc.element.pino.tools.copy)
- description and source-code
```javascript
function copy(a, b) {
  for (var k in b) { a[k] = b[k] }
  return a
}
```
- example usage
```shell
...

Object.defineProperty(pinoPrototype, 'level', {
  get: pinoPrototype._getLevel,
  set: pinoPrototype._setLevel
})

Object.defineProperty(pinoPrototype, '_lscache', {
  value: tools.copy({}, levels.lscache)
})

Object.defineProperty(
  pinoPrototype,
  'LOG_VERSION',
  {value: LOG_VERSION}
)
...
```

#### <a name="apidoc.element.pino.tools.defineLevelsProperty"></a>[function <span class="apidocSignatureSpan">pino.tools.</span>defineLevelsProperty (onObject)](#apidoc.element.pino.tools.defineLevelsProperty)
- description and source-code
```javascript
function defineLevelsProperty(onObject) {
  Object.defineProperty(onObject, 'levels', {
    value: {
      values: copy({}, levels.levels),
      labels: copy({}, levels.nums)
    },
    enumerable: true
  })
  Object.defineProperty(onObject.levels.values, 'silent', {value: Infinity})
  Object.defineProperty(onObject.levels.labels, Infinity, {value: 'silent'})
}
```
- example usage
```shell
...

if (iopts.enabled === false) {
  iopts.level = 'silent'
}

var instance = Object.create(pinoPrototype)
instance.stream = istream
tools.defineLevelsProperty(instance)
tools.applyOptions.call(instance, iopts)
if (iopts.cache) setTimeout(waitForFDSettle, 100)

var settleTries = 0
function waitForFDSettle () {
  var isBlockable = tools.streamIsBlockable(istream)
  if (isBlockable === false && settleTries > 10) {
...
```

#### <a name="apidoc.element.pino.tools.genLog"></a>[function <span class="apidocSignatureSpan">pino.tools.</span>genLog (z)](#apidoc.element.pino.tools.genLog)
- description and source-code
```javascript
function genLog(z) {
  return function LOG (a, b, c, d, e, f, g, h, i, j, k) {
    var l = 0
    var m = null
    var n = null
    var o
    var p
    if (typeof a === 'object' && a !== null) {
      m = a
      n = [b, c, d, e, f, g, h, i, j, k]
      l = 1

      if (m.method && m.headers && m.socket) {
        m = serializers.mapHttpRequest(m)
      } else if (typeof m.setHeader === 'function') {
        m = serializers.mapHttpResponse(m)
      }
    } else {
      n = [a, b, c, d, e, f, g, h, i, j, k]
    }
    p = n.length = arguments.length - l
    if (p > 1) {
      l = typeof a === 'string' ? countInterp(a, '%j') : 0
      if (l) {
        n.length = l + countInterp(a, '%d') + countInterp(a, '%s') + 1
        o = '${util.format.apply(null, n)}'
      } else {
        o = format(n, this.formatOpts)
      }
    } else if (p) {
      o = n[0]
    }
    this.write(m, o, z)
  }
}
```
- example usage
```shell
...
  writable: true
}
})

var levelMethods = ['fatal', 'error', 'warn', 'info', 'debug', 'trace']
levelMethods.forEach(function (m) {
Object.defineProperty(pinoPrototype, m, {
  value: tools.genLog(levels.levels[m]),
  enumerable: true,
  writable: true
})
})

function getLevelVal () {
return this._levelVal
...
```

#### <a name="apidoc.element.pino.tools.noop"></a>[function <span class="apidocSignatureSpan">pino.tools.</span>noop ()](#apidoc.element.pino.tools.noop)
- description and source-code
```javascript
function noop() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pino.tools.streamIsBlockable"></a>[function <span class="apidocSignatureSpan">pino.tools.</span>streamIsBlockable (s)](#apidoc.element.pino.tools.streamIsBlockable)
- description and source-code
```javascript
function streamIsBlockable(s) {
  if (s.hasOwnProperty('_handle') && s._handle.hasOwnProperty('fd') && s._handle.fd) return true
  if (s.hasOwnProperty('fd') && s.fd) return true
  return false
}
```
- example usage
```shell
...
instance.stream = istream
tools.defineLevelsProperty(instance)
tools.applyOptions.call(instance, iopts)
if (iopts.cache) setTimeout(waitForFDSettle, 100)

var settleTries = 0
function waitForFDSettle () {
  var isBlockable = tools.streamIsBlockable(istream)
  if (isBlockable === false && settleTries > 10) {
    return instance.emit('error', Error('stream must have a file descriptor in extreme mode'))
  } else if (isBlockable === true) {
    return events(instance, extremeModeExitHandler)
  }
  settleTries += 1
  setTimeout(waitForFDSettle, 100)
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
