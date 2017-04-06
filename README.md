# api documentation for  [faye-websocket (v0.11.1)](https://github.com/faye/faye-websocket-node)  [![npm package](https://img.shields.io/npm/v/npmdoc-faye-websocket.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-faye-websocket) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-faye-websocket.svg)](https://travis-ci.org/npmdoc/node-npmdoc-faye-websocket)
#### Standards-compliant WebSocket server and client

[![NPM](https://nodei.co/npm/faye-websocket.png?downloads=true)](https://www.npmjs.com/package/faye-websocket)

[![apidoc](https://npmdoc.github.io/node-npmdoc-faye-websocket/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-faye-websocket_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-faye-websocket/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-faye-websocket/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-faye-websocket/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "James Coglan",
        "email": "jcoglan@gmail.com",
        "url": "http://jcoglan.com/"
    },
    "bugs": {
        "url": "https://github.com/faye/faye-websocket-node/issues"
    },
    "dependencies": {
        "websocket-driver": ">=0.5.1"
    },
    "description": "Standards-compliant WebSocket server and client",
    "devDependencies": {
        "jstest": "",
        "pace": "",
        "permessage-deflate": ""
    },
    "directories": {},
    "dist": {
        "shasum": "f0efe18c4f56e4f40afc7e06c719fd5ee6188f38",
        "tarball": "https://registry.npmjs.org/faye-websocket/-/faye-websocket-0.11.1.tgz"
    },
    "engines": {
        "node": ">=0.8.0"
    },
    "gitHead": "49eab191cc2946e40bdee650e9bd0bb2384562a2",
    "homepage": "https://github.com/faye/faye-websocket-node",
    "keywords": [
        "websocket",
        "eventsource"
    ],
    "license": "MIT",
    "main": "./lib/faye/websocket",
    "maintainers": [
        {
            "name": "jcoglan",
            "email": "jcoglan@gmail.com"
        }
    ],
    "name": "faye-websocket",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/faye/faye-websocket-node.git"
    },
    "scripts": {
        "test": "jstest spec/runner.js"
    },
    "version": "0.11.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module faye-websocket](#apidoc.module.faye-websocket)
1.  [function <span class="apidocSignatureSpan">faye-websocket.</span>Client (_url, protocols, options)](#apidoc.element.faye-websocket.Client)
1.  [function <span class="apidocSignatureSpan">faye-websocket.</span>EventSource (request, response, options)](#apidoc.element.faye-websocket.EventSource)
1.  [function <span class="apidocSignatureSpan">faye-websocket.</span>WebSocket (request, socket, body, protocols, options)](#apidoc.element.faye-websocket.WebSocket)
1.  [function <span class="apidocSignatureSpan">faye-websocket.</span>isWebSocket (request)](#apidoc.element.faye-websocket.isWebSocket)
1.  [function <span class="apidocSignatureSpan">faye-websocket.</span>super_ (options)](#apidoc.element.faye-websocket.super_)
1.  [function <span class="apidocSignatureSpan">faye-websocket.</span>validateOptions (options, validKeys)](#apidoc.element.faye-websocket.validateOptions)
1.  object <span class="apidocSignatureSpan">faye-websocket.</span>Client.prototype
1.  object <span class="apidocSignatureSpan">faye-websocket.</span>EventSource.prototype
1.  object <span class="apidocSignatureSpan">faye-websocket.</span>super_.prototype

#### [module faye-websocket.Client](#apidoc.module.faye-websocket.Client)
1.  [function <span class="apidocSignatureSpan">faye-websocket.</span>Client (_url, protocols, options)](#apidoc.element.faye-websocket.Client.Client)
1.  [function <span class="apidocSignatureSpan">faye-websocket.Client.</span>super_ (options)](#apidoc.element.faye-websocket.Client.super_)

#### [module faye-websocket.Client.prototype](#apidoc.module.faye-websocket.Client.prototype)
1.  [function <span class="apidocSignatureSpan">faye-websocket.Client.prototype.</span>_configureProxy (proxy, originTLS)](#apidoc.element.faye-websocket.Client.prototype._configureProxy)
1.  [function <span class="apidocSignatureSpan">faye-websocket.Client.prototype.</span>_onConnect ()](#apidoc.element.faye-websocket.Client.prototype._onConnect)

#### [module faye-websocket.EventSource](#apidoc.module.faye-websocket.EventSource)
1.  [function <span class="apidocSignatureSpan">faye-websocket.</span>EventSource (request, response, options)](#apidoc.element.faye-websocket.EventSource.EventSource)
1.  [function <span class="apidocSignatureSpan">faye-websocket.EventSource.</span>isEventSource (request)](#apidoc.element.faye-websocket.EventSource.isEventSource)
1.  [function <span class="apidocSignatureSpan">faye-websocket.EventSource.</span>super_ ()](#apidoc.element.faye-websocket.EventSource.super_)

#### [module faye-websocket.EventSource.prototype](#apidoc.module.faye-websocket.EventSource.prototype)
1.  [function <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>_open ()](#apidoc.element.faye-websocket.EventSource.prototype._open)
1.  [function <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>_write (chunk)](#apidoc.element.faye-websocket.EventSource.prototype._write)
1.  [function <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>addEventListener (eventType, listener, useCapture)](#apidoc.element.faye-websocket.EventSource.prototype.addEventListener)
1.  [function <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>close ()](#apidoc.element.faye-websocket.EventSource.prototype.close)
1.  [function <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>dispatchEvent (event)](#apidoc.element.faye-websocket.EventSource.prototype.dispatchEvent)
1.  [function <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>end (message)](#apidoc.element.faye-websocket.EventSource.prototype.end)
1.  [function <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>ping ()](#apidoc.element.faye-websocket.EventSource.prototype.ping)
1.  [function <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>removeEventListener (eventType, listener, useCapture)](#apidoc.element.faye-websocket.EventSource.prototype.removeEventListener)
1.  [function <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>send (message, options)](#apidoc.element.faye-websocket.EventSource.prototype.send)
1.  [function <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>write (message)](#apidoc.element.faye-websocket.EventSource.prototype.write)
1.  number <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>DEFAULT_PING
1.  number <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>DEFAULT_RETRY
1.  object <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>onclose
1.  object <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>onerror
1.  object <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>onmessage
1.  object <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>onopen

#### [module faye-websocket.super_](#apidoc.module.faye-websocket.super_)
1.  [function <span class="apidocSignatureSpan">faye-websocket.</span>super_ ()](#apidoc.element.faye-websocket.super_.super_)
1.  number <span class="apidocSignatureSpan">faye-websocket.super_.</span>CLOSED
1.  number <span class="apidocSignatureSpan">faye-websocket.super_.</span>CLOSE_TIMEOUT
1.  number <span class="apidocSignatureSpan">faye-websocket.super_.</span>CLOSING
1.  number <span class="apidocSignatureSpan">faye-websocket.super_.</span>CONNECTING
1.  number <span class="apidocSignatureSpan">faye-websocket.super_.</span>OPEN

#### [module faye-websocket.super_.prototype](#apidoc.module.faye-websocket.super_.prototype)
1.  [function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>_beginClose (reason, code)](#apidoc.element.faye-websocket.super_.prototype._beginClose)
1.  [function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>_configureStream ()](#apidoc.element.faye-websocket.super_.prototype._configureStream)
1.  [function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>_emitError (message)](#apidoc.element.faye-websocket.super_.prototype._emitError)
1.  [function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>_finalizeClose ()](#apidoc.element.faye-websocket.super_.prototype._finalizeClose)
1.  [function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>_open ()](#apidoc.element.faye-websocket.super_.prototype._open)
1.  [function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>_receiveMessage (data)](#apidoc.element.faye-websocket.super_.prototype._receiveMessage)
1.  [function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>addEventListener (eventType, listener, useCapture)](#apidoc.element.faye-websocket.super_.prototype.addEventListener)
1.  [function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>close (code, reason)](#apidoc.element.faye-websocket.super_.prototype.close)
1.  [function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>dispatchEvent (event)](#apidoc.element.faye-websocket.super_.prototype.dispatchEvent)
1.  [function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>end (data)](#apidoc.element.faye-websocket.super_.prototype.end)
1.  [function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>pause ()](#apidoc.element.faye-websocket.super_.prototype.pause)
1.  [function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>ping (message, callback)](#apidoc.element.faye-websocket.super_.prototype.ping)
1.  [function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>removeEventListener (eventType, listener, useCapture)](#apidoc.element.faye-websocket.super_.prototype.removeEventListener)
1.  [function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>resume ()](#apidoc.element.faye-websocket.super_.prototype.resume)
1.  [function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>send (data)](#apidoc.element.faye-websocket.super_.prototype.send)
1.  [function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>write (data)](#apidoc.element.faye-websocket.super_.prototype.write)
1.  object <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>onclose
1.  object <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>onerror
1.  object <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>onmessage
1.  object <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>onopen



# <a name="apidoc.module.faye-websocket"></a>[module faye-websocket](#apidoc.module.faye-websocket)

#### <a name="apidoc.element.faye-websocket.Client"></a>[function <span class="apidocSignatureSpan">faye-websocket.</span>Client (_url, protocols, options)](#apidoc.element.faye-websocket.Client)
- description and source-code
```javascript
Client = function (_url, protocols, options) {
  options = options || {};

  this.url     = _url;
  this._driver = driver.client(this.url, {maxLength: options.maxLength, protocols: protocols});

  ['open', 'error'].forEach(function(event) {
    this._driver.on(event, function() {
      self.headers    = self._driver.headers;
      self.statusCode = self._driver.statusCode;
    });
  }, this);

  var proxy      = options.proxy || {},
      endpoint   = url.parse(proxy.origin || this.url),
      port       = endpoint.port || DEFAULT_PORTS[endpoint.protocol],
      secure     = SECURE_PROTOCOLS.indexOf(endpoint.protocol) >= 0,
      onConnect  = function() { self._onConnect() },
      netOptions = options.net || {},
      originTLS  = options.tls || {},
      socketTLS  = proxy.origin ? (proxy.tls || {}) : originTLS,
      self       = this;

  netOptions.host = socketTLS.host = endpoint.hostname;
  netOptions.port = socketTLS.port = port;

  originTLS.ca = originTLS.ca || options.ca;
  socketTLS.servername = socketTLS.servername || endpoint.hostname;

  this._stream = secure
               ? tls.connect(socketTLS, onConnect)
               : net.connect(netOptions, onConnect);

  if (proxy.origin) this._configureProxy(proxy, originTLS);

  API.call(this, options);
}
```
- example usage
```shell
...

The client supports both the plain-text 'ws' protocol and the encrypted 'wss'
protocol, and has exactly the same interface as a socket you would use in a web
browser. On the wire it identifies itself as 'hybi-13'.

'''js
var WebSocket = require('faye-websocket'),
    ws        = new WebSocket.Client('ws://www.example.com/');

ws.on('open', function(event) {
  console.log('open');
  ws.send('Hello, world!');
});

ws.on('message', function(event) {
...
```

#### <a name="apidoc.element.faye-websocket.EventSource"></a>[function <span class="apidocSignatureSpan">faye-websocket.</span>EventSource (request, response, options)](#apidoc.element.faye-websocket.EventSource)
- description and source-code
```javascript
EventSource = function (request, response, options) {
  this.writable = true;
  options = options || {};

  this._stream = response.socket;
  this._ping   = options.ping  || this.DEFAULT_PING;
  this._retry  = options.retry || this.DEFAULT_RETRY;

  var scheme       = driver.isSecureRequest(request) ? 'https:' : 'http:';
  this.url         = scheme + '//' + request.headers.host + request.url;
  this.lastEventId = request.headers['last-event-id'] || '';
  this.readyState  = API.CONNECTING;

  var headers = new Headers(),
      self    = this;

  if (options.headers) {
    for (var key in options.headers) headers.set(key, options.headers[key]);
  }

  if (!this._stream || !this._stream.writable) return;
  process.nextTick(function() { self._open() });

  this._stream.setTimeout(0);
  this._stream.setNoDelay(true);

  var handshake = 'HTTP/1.1 200 OK\r\n' +
                  'Content-Type: text/event-stream\r\n' +
                  'Cache-Control: no-cache, no-store\r\n' +
                  'Connection: close\r\n' +
                  headers.toString() +
                  '\r\n' +
                  'retry: ' + Math.floor(this._retry * 1000) + '\r\n\r\n';

  this._write(handshake);

  this._stream.on('drain', function() { self.emit('drain') });

  if (this._ping)
    this._pingTimer = setInterval(function() { self.ping() }, this._ping * 1000);

  ['error', 'end'].forEach(function(event) {
    self._stream.on(event, function() { self.close() });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.WebSocket"></a>[function <span class="apidocSignatureSpan">faye-websocket.</span>WebSocket (request, socket, body, protocols, options)](#apidoc.element.faye-websocket.WebSocket)
- description and source-code
```javascript
WebSocket = function (request, socket, body, protocols, options) {
  options = options || {};

  this._stream = socket;
  this._driver = driver.http(request, {maxLength: options.maxLength, protocols: protocols});

  var self = this;
  if (!this._stream || !this._stream.writable) return;
  if (!this._stream.readable) return this._stream.end();

  var catchup = function() { self._stream.removeListener('data', catchup) };
  this._stream.on('data', catchup);

  API.call(this, options);

  process.nextTick(function() {
    self._driver.start();
    self._driver.io.write(body);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.isWebSocket"></a>[function <span class="apidocSignatureSpan">faye-websocket.</span>isWebSocket (request)](#apidoc.element.faye-websocket.isWebSocket)
- description and source-code
```javascript
isWebSocket = function (request) {
  return driver.isWebSocket(request);
}
```
- example usage
```shell
...
'''js
var WebSocket = require('faye-websocket'),
  http      = require('http');

var server = http.createServer();

server.on('upgrade', function(request, socket, body) {
if (WebSocket.isWebSocket(request)) {
  var ws = new WebSocket(request, socket, body);

  ws.on('message', function(event) {
    ws.send(event.data);
  });

  ws.on('close', function(event) {
...
```

#### <a name="apidoc.element.faye-websocket.super_"></a>[function <span class="apidocSignatureSpan">faye-websocket.</span>super_ (options)](#apidoc.element.faye-websocket.super_)
- description and source-code
```javascript
super_ = function (options) {
  options = options || {};
  driver.validateOptions(options, ['headers', 'extensions', 'maxLength', 'ping', 'proxy', 'tls', 'ca']);

  this.readable = this.writable = true;

  var headers = options.headers;
  if (headers) {
    for (var name in headers) this._driver.setHeader(name, headers[name]);
  }

  var extensions = options.extensions;
  if (extensions) {
    [].concat(extensions).forEach(this._driver.addExtension, this._driver);
  }

  this._ping          = options.ping;
  this._pingId        = 0;
  this.readyState     = API.CONNECTING;
  this.bufferedAmount = 0;
  this.protocol       = '';
  this.url            = this._driver.url;
  this.version        = this._driver.version;

  var self = this;

  this._driver.on('open',    function(e) { self._open() });
  this._driver.on('message', function(e) { self._receiveMessage(e.data) });
  this._driver.on('close',   function(e) { self._beginClose(e.reason, e.code) });

  this._driver.on('error', function(error) {
    self._emitError(error.message);
  });
  this.on('error', function() {});

  this._driver.messages.on('drain', function() {
    self.emit('drain');
  });

  if (this._ping)
    this._pingTimer = setInterval(function() {
      self._pingId += 1;
      self.ping(self._pingId.toString());
    }, this._ping * 1000);

  this._configureStream();

  if (!this._proxy) {
    this._stream.pipe(this._driver.io);
    this._driver.io.pipe(this._stream);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.validateOptions"></a>[function <span class="apidocSignatureSpan">faye-websocket.</span>validateOptions (options, validKeys)](#apidoc.element.faye-websocket.validateOptions)
- description and source-code
```javascript
validateOptions = function (options, validKeys) {
  driver.validateOptions(options, validKeys);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.faye-websocket.Client"></a>[module faye-websocket.Client](#apidoc.module.faye-websocket.Client)

#### <a name="apidoc.element.faye-websocket.Client.Client"></a>[function <span class="apidocSignatureSpan">faye-websocket.</span>Client (_url, protocols, options)](#apidoc.element.faye-websocket.Client.Client)
- description and source-code
```javascript
Client = function (_url, protocols, options) {
  options = options || {};

  this.url     = _url;
  this._driver = driver.client(this.url, {maxLength: options.maxLength, protocols: protocols});

  ['open', 'error'].forEach(function(event) {
    this._driver.on(event, function() {
      self.headers    = self._driver.headers;
      self.statusCode = self._driver.statusCode;
    });
  }, this);

  var proxy      = options.proxy || {},
      endpoint   = url.parse(proxy.origin || this.url),
      port       = endpoint.port || DEFAULT_PORTS[endpoint.protocol],
      secure     = SECURE_PROTOCOLS.indexOf(endpoint.protocol) >= 0,
      onConnect  = function() { self._onConnect() },
      netOptions = options.net || {},
      originTLS  = options.tls || {},
      socketTLS  = proxy.origin ? (proxy.tls || {}) : originTLS,
      self       = this;

  netOptions.host = socketTLS.host = endpoint.hostname;
  netOptions.port = socketTLS.port = port;

  originTLS.ca = originTLS.ca || options.ca;
  socketTLS.servername = socketTLS.servername || endpoint.hostname;

  this._stream = secure
               ? tls.connect(socketTLS, onConnect)
               : net.connect(netOptions, onConnect);

  if (proxy.origin) this._configureProxy(proxy, originTLS);

  API.call(this, options);
}
```
- example usage
```shell
...

The client supports both the plain-text 'ws' protocol and the encrypted 'wss'
protocol, and has exactly the same interface as a socket you would use in a web
browser. On the wire it identifies itself as 'hybi-13'.

'''js
var WebSocket = require('faye-websocket'),
    ws        = new WebSocket.Client('ws://www.example.com/');

ws.on('open', function(event) {
  console.log('open');
  ws.send('Hello, world!');
});

ws.on('message', function(event) {
...
```

#### <a name="apidoc.element.faye-websocket.Client.super_"></a>[function <span class="apidocSignatureSpan">faye-websocket.Client.</span>super_ (options)](#apidoc.element.faye-websocket.Client.super_)
- description and source-code
```javascript
super_ = function (options) {
  options = options || {};
  driver.validateOptions(options, ['headers', 'extensions', 'maxLength', 'ping', 'proxy', 'tls', 'ca']);

  this.readable = this.writable = true;

  var headers = options.headers;
  if (headers) {
    for (var name in headers) this._driver.setHeader(name, headers[name]);
  }

  var extensions = options.extensions;
  if (extensions) {
    [].concat(extensions).forEach(this._driver.addExtension, this._driver);
  }

  this._ping          = options.ping;
  this._pingId        = 0;
  this.readyState     = API.CONNECTING;
  this.bufferedAmount = 0;
  this.protocol       = '';
  this.url            = this._driver.url;
  this.version        = this._driver.version;

  var self = this;

  this._driver.on('open',    function(e) { self._open() });
  this._driver.on('message', function(e) { self._receiveMessage(e.data) });
  this._driver.on('close',   function(e) { self._beginClose(e.reason, e.code) });

  this._driver.on('error', function(error) {
    self._emitError(error.message);
  });
  this.on('error', function() {});

  this._driver.messages.on('drain', function() {
    self.emit('drain');
  });

  if (this._ping)
    this._pingTimer = setInterval(function() {
      self._pingId += 1;
      self.ping(self._pingId.toString());
    }, this._ping * 1000);

  this._configureStream();

  if (!this._proxy) {
    this._stream.pipe(this._driver.io);
    this._driver.io.pipe(this._stream);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.faye-websocket.Client.prototype"></a>[module faye-websocket.Client.prototype](#apidoc.module.faye-websocket.Client.prototype)

#### <a name="apidoc.element.faye-websocket.Client.prototype._configureProxy"></a>[function <span class="apidocSignatureSpan">faye-websocket.Client.prototype.</span>_configureProxy (proxy, originTLS)](#apidoc.element.faye-websocket.Client.prototype._configureProxy)
- description and source-code
```javascript
_configureProxy = function (proxy, originTLS) {
  var uri    = url.parse(this.url),
      secure = SECURE_PROTOCOLS.indexOf(uri.protocol) >= 0,
      self   = this,
      name;

  this._proxy = this._driver.proxy(proxy.origin);

  if (proxy.headers) {
    for (name in proxy.headers) this._proxy.setHeader(name, proxy.headers[name]);
  }

  this._proxy.pipe(this._stream, {end: false});
  this._stream.pipe(this._proxy);

  this._proxy.on('connect', function() {
    if (secure) {
      var options = {socket: self._stream, servername: uri.hostname};
      for (name in originTLS) options[name] = originTLS[name];
      self._stream = tls.connect(options);
      self._configureStream();
    }
    self._driver.io.pipe(self._stream);
    self._stream.pipe(self._driver.io);
    self._driver.start();
  });

  this._proxy.on('error', function(error) {
    self._driver.emit('error', error);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.Client.prototype._onConnect"></a>[function <span class="apidocSignatureSpan">faye-websocket.Client.prototype.</span>_onConnect ()](#apidoc.element.faye-websocket.Client.prototype._onConnect)
- description and source-code
```javascript
_onConnect = function () {
  var worker = this._proxy || this._driver;
  worker.start();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.faye-websocket.EventSource"></a>[module faye-websocket.EventSource](#apidoc.module.faye-websocket.EventSource)

#### <a name="apidoc.element.faye-websocket.EventSource.EventSource"></a>[function <span class="apidocSignatureSpan">faye-websocket.</span>EventSource (request, response, options)](#apidoc.element.faye-websocket.EventSource.EventSource)
- description and source-code
```javascript
EventSource = function (request, response, options) {
  this.writable = true;
  options = options || {};

  this._stream = response.socket;
  this._ping   = options.ping  || this.DEFAULT_PING;
  this._retry  = options.retry || this.DEFAULT_RETRY;

  var scheme       = driver.isSecureRequest(request) ? 'https:' : 'http:';
  this.url         = scheme + '//' + request.headers.host + request.url;
  this.lastEventId = request.headers['last-event-id'] || '';
  this.readyState  = API.CONNECTING;

  var headers = new Headers(),
      self    = this;

  if (options.headers) {
    for (var key in options.headers) headers.set(key, options.headers[key]);
  }

  if (!this._stream || !this._stream.writable) return;
  process.nextTick(function() { self._open() });

  this._stream.setTimeout(0);
  this._stream.setNoDelay(true);

  var handshake = 'HTTP/1.1 200 OK\r\n' +
                  'Content-Type: text/event-stream\r\n' +
                  'Cache-Control: no-cache, no-store\r\n' +
                  'Connection: close\r\n' +
                  headers.toString() +
                  '\r\n' +
                  'retry: ' + Math.floor(this._retry * 1000) + '\r\n\r\n';

  this._write(handshake);

  this._stream.on('drain', function() { self.emit('drain') });

  if (this._ping)
    this._pingTimer = setInterval(function() { self.ping() }, this._ping * 1000);

  ['error', 'end'].forEach(function(event) {
    self._stream.on(event, function() { self.close() });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.EventSource.isEventSource"></a>[function <span class="apidocSignatureSpan">faye-websocket.EventSource.</span>isEventSource (request)](#apidoc.element.faye-websocket.EventSource.isEventSource)
- description and source-code
```javascript
isEventSource = function (request) {
  if (request.method !== 'GET') return false;
  var accept = (request.headers.accept || '').split(/\s*,\s*/);
  return accept.indexOf('text/event-stream') >= 0;
}
```
- example usage
```shell
...
var WebSocket   = require('faye-websocket'),
  EventSource = WebSocket.EventSource,
  http        = require('http');

var server = http.createServer();

server.on('request', function(request, response) {
if (EventSource.isEventSource(request)) {
  var es = new EventSource(request, response);
  console.log('open', es.url, es.lastEventId);

  // Periodically send messages
  var loop = setInterval(function() { es.send('Hello') }, 1000);

  es.on('close', function() {
...
```

#### <a name="apidoc.element.faye-websocket.EventSource.super_"></a>[function <span class="apidocSignatureSpan">faye-websocket.EventSource.</span>super_ ()](#apidoc.element.faye-websocket.EventSource.super_)
- description and source-code
```javascript
function Stream() {
  EE.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.faye-websocket.EventSource.prototype"></a>[module faye-websocket.EventSource.prototype](#apidoc.module.faye-websocket.EventSource.prototype)

#### <a name="apidoc.element.faye-websocket.EventSource.prototype._open"></a>[function <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>_open ()](#apidoc.element.faye-websocket.EventSource.prototype._open)
- description and source-code
```javascript
_open = function () {
  if (this.readyState !== API.CONNECTING) return;

  this.readyState = API.OPEN;

  var event = new Event('open');
  event.initEvent('open', false, false);
  this.dispatchEvent(event);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.EventSource.prototype._write"></a>[function <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>_write (chunk)](#apidoc.element.faye-websocket.EventSource.prototype._write)
- description and source-code
```javascript
_write = function (chunk) {
  if (!this.writable) return false;
  try {
    return this._stream.write(chunk, 'utf8');
  } catch (e) {
    return false;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.EventSource.prototype.addEventListener"></a>[function <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>addEventListener (eventType, listener, useCapture)](#apidoc.element.faye-websocket.EventSource.prototype.addEventListener)
- description and source-code
```javascript
addEventListener = function (eventType, listener, useCapture) {
  this.on(eventType, listener);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.EventSource.prototype.close"></a>[function <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>close ()](#apidoc.element.faye-websocket.EventSource.prototype.close)
- description and source-code
```javascript
close = function () {
  if (this.readyState > API.OPEN) return false;

  this.readyState = API.CLOSED;
  this.writable = false;
  if (this._pingTimer) clearInterval(this._pingTimer);
  if (this._stream) this._stream.end();

  var event = new Event('close');
  event.initEvent('close', false, false);
  this.dispatchEvent(event);

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.EventSource.prototype.dispatchEvent"></a>[function <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>dispatchEvent (event)](#apidoc.element.faye-websocket.EventSource.prototype.dispatchEvent)
- description and source-code
```javascript
dispatchEvent = function (event) {
  event.target = event.currentTarget = this;
  event.eventPhase = Event.AT_TARGET;

  if (this['on' + event.type])
    this['on' + event.type](event);

  this.emit(event.type, event);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.EventSource.prototype.end"></a>[function <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>end (message)](#apidoc.element.faye-websocket.EventSource.prototype.end)
- description and source-code
```javascript
end = function (message) {
  if (message !== undefined) this.write(message);
  this.close();
}
```
- example usage
```shell
...
      clearInterval(loop);
      es = null;
    });

  } else {
    // Normal HTTP request
    response.writeHead(200, {'Content-Type': 'text/plain'});
    response.end('Hello');
  }
});

server.listen(8000);
'''

The 'send' method takes two optional parameters, 'event' and 'id'. The default
...
```

#### <a name="apidoc.element.faye-websocket.EventSource.prototype.ping"></a>[function <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>ping ()](#apidoc.element.faye-websocket.EventSource.prototype.ping)
- description and source-code
```javascript
ping = function () {
  return this._write(':\r\n\r\n');
}
```
- example usage
```shell
...
handshake from the client yet. In this case, calls to 'ws.send()' will buffer
the message in memory until the handshake is complete, at which point any
buffered messages will be sent to the client.

If you need to detect when the WebSocket handshake is complete, you can use the
'onopen' event.

If the connection's protocol version supports it, you can call 'ws.ping()' to
send a ping message and wait for the client's response. This method takes a
message string, and an optional callback that fires when a matching pong message
is received. It returns 'true' if and only if a ping message was sent. If the
client does not support ping/pong, this method sends no data and returns
'false'.

'''js
...
```

#### <a name="apidoc.element.faye-websocket.EventSource.prototype.removeEventListener"></a>[function <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>removeEventListener (eventType, listener, useCapture)](#apidoc.element.faye-websocket.EventSource.prototype.removeEventListener)
- description and source-code
```javascript
removeEventListener = function (eventType, listener, useCapture) {
  this.removeListener(eventType, listener);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.EventSource.prototype.send"></a>[function <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>send (message, options)](#apidoc.element.faye-websocket.EventSource.prototype.send)
- description and source-code
```javascript
send = function (message, options) {
  if (this.readyState > API.OPEN) return false;

  message = String(message).replace(/(\r\n|\r|\n)/g, '$1data: ');
  options = options || {};

  var frame = '';
  if (options.event) frame += 'event: ' + options.event + '\r\n';
  if (options.id)    frame += 'id: '    + options.id    + '\r\n';
  frame += 'data: ' + message + '\r\n\r\n';

  return this._write(frame);
}
```
- example usage
```shell
...
var server = http.createServer();

server.on('upgrade', function(request, socket, body) {
if (WebSocket.isWebSocket(request)) {
  var ws = new WebSocket(request, socket, body);

  ws.on('message', function(event) {
    ws.send(event.data);
  });

  ws.on('close', function(event) {
    console.log('close', event.code, event.reason);
    ws = null;
  });
}
...
```

#### <a name="apidoc.element.faye-websocket.EventSource.prototype.write"></a>[function <span class="apidocSignatureSpan">faye-websocket.EventSource.prototype.</span>write (message)](#apidoc.element.faye-websocket.EventSource.prototype.write)
- description and source-code
```javascript
write = function (message) {
  return this.send(message);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.faye-websocket.super_"></a>[module faye-websocket.super_](#apidoc.module.faye-websocket.super_)

#### <a name="apidoc.element.faye-websocket.super_.super_"></a>[function <span class="apidocSignatureSpan">faye-websocket.</span>super_ ()](#apidoc.element.faye-websocket.super_.super_)
- description and source-code
```javascript
function Stream() {
  EE.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.faye-websocket.super_.prototype"></a>[module faye-websocket.super_.prototype](#apidoc.module.faye-websocket.super_.prototype)

#### <a name="apidoc.element.faye-websocket.super_.prototype._beginClose"></a>[function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>_beginClose (reason, code)](#apidoc.element.faye-websocket.super_.prototype._beginClose)
- description and source-code
```javascript
_beginClose = function (reason, code) {
  if (this.readyState === API.CLOSED) return;
  this.readyState = API.CLOSING;
  this._closeParams = [reason, code];

  if (this._stream) {
    this._stream.destroy();
    if (!this._stream.readable) this._finalizeClose();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.super_.prototype._configureStream"></a>[function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>_configureStream ()](#apidoc.element.faye-websocket.super_.prototype._configureStream)
- description and source-code
```javascript
_configureStream = function () {
  var self = this;

  this._stream.setTimeout(0);
  this._stream.setNoDelay(true);

  ['close', 'end'].forEach(function(event) {
    this._stream.on(event, function() { self._finalizeClose() });
  }, this);

  this._stream.on('error', function(error) {
    self._emitError('Network error: ' + self.url + ': ' + error.message);
    self._finalizeClose();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.super_.prototype._emitError"></a>[function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>_emitError (message)](#apidoc.element.faye-websocket.super_.prototype._emitError)
- description and source-code
```javascript
_emitError = function (message) {
  if (this.readyState >= API.CLOSING) return;

  var event = new Event('error', {message: message});
  event.initEvent('error', false, false);
  this.dispatchEvent(event);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.super_.prototype._finalizeClose"></a>[function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>_finalizeClose ()](#apidoc.element.faye-websocket.super_.prototype._finalizeClose)
- description and source-code
```javascript
_finalizeClose = function () {
  if (this.readyState === API.CLOSED) return;
  this.readyState = API.CLOSED;

  if (this._closeTimer) clearTimeout(this._closeTimer);
  if (this._pingTimer) clearInterval(this._pingTimer);
  if (this._stream) this._stream.end();

  if (this.readable) this.emit('end');
  this.readable = this.writable = false;

  var reason = this._closeParams ? this._closeParams[0] : '',
      code   = this._closeParams ? this._closeParams[1] : 1006;

  var event = new Event('close', {code: code, reason: reason});
  event.initEvent('close', false, false);
  this.dispatchEvent(event);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.super_.prototype._open"></a>[function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>_open ()](#apidoc.element.faye-websocket.super_.prototype._open)
- description and source-code
```javascript
_open = function () {
  if (this.readyState !== API.CONNECTING) return;

  this.readyState = API.OPEN;
  this.protocol = this._driver.protocol || '';

  var event = new Event('open');
  event.initEvent('open', false, false);
  this.dispatchEvent(event);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.super_.prototype._receiveMessage"></a>[function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>_receiveMessage (data)](#apidoc.element.faye-websocket.super_.prototype._receiveMessage)
- description and source-code
```javascript
_receiveMessage = function (data) {
  if (this.readyState > API.OPEN) return false;

  if (this.readable) this.emit('data', data);

  var event = new Event('message', {data: data});
  event.initEvent('message', false, false);
  this.dispatchEvent(event);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.super_.prototype.addEventListener"></a>[function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>addEventListener (eventType, listener, useCapture)](#apidoc.element.faye-websocket.super_.prototype.addEventListener)
- description and source-code
```javascript
addEventListener = function (eventType, listener, useCapture) {
  this.on(eventType, listener);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.super_.prototype.close"></a>[function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>close (code, reason)](#apidoc.element.faye-websocket.super_.prototype.close)
- description and source-code
```javascript
close = function (code, reason) {
  if (code === undefined) code = 1000;
  if (reason === undefined) reason = '';

  if (code !== 1000 && (code < 3000 || code > 4999))
    throw new Error("Failed to execute 'close' on WebSocket: " +
                    "The code must be either 1000, or between 3000 and 4999. " +
                    code + " is neither.");

  if (this.readyState !== API.CLOSED) this.readyState = API.CLOSING;
  this._driver.close(reason, code);

  var self = this;

  this._closeTimer = setTimeout(function() {
    self._beginClose('', 1006);
  }, API.CLOSE_TIMEOUT);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.super_.prototype.dispatchEvent"></a>[function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>dispatchEvent (event)](#apidoc.element.faye-websocket.super_.prototype.dispatchEvent)
- description and source-code
```javascript
dispatchEvent = function (event) {
  event.target = event.currentTarget = this;
  event.eventPhase = Event.AT_TARGET;

  if (this['on' + event.type])
    this['on' + event.type](event);

  this.emit(event.type, event);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.super_.prototype.end"></a>[function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>end (data)](#apidoc.element.faye-websocket.super_.prototype.end)
- description and source-code
```javascript
end = function (data) {
  if (data !== undefined) this.send(data);
  this.close();
}
```
- example usage
```shell
...
      clearInterval(loop);
      es = null;
    });

  } else {
    // Normal HTTP request
    response.writeHead(200, {'Content-Type': 'text/plain'});
    response.end('Hello');
  }
});

server.listen(8000);
'''

The 'send' method takes two optional parameters, 'event' and 'id'. The default
...
```

#### <a name="apidoc.element.faye-websocket.super_.prototype.pause"></a>[function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>pause ()](#apidoc.element.faye-websocket.super_.prototype.pause)
- description and source-code
```javascript
pause = function () {
  return this._driver.messages.pause();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.super_.prototype.ping"></a>[function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>ping (message, callback)](#apidoc.element.faye-websocket.super_.prototype.ping)
- description and source-code
```javascript
ping = function (message, callback) {
  if (this.readyState > API.OPEN) return false;
  return this._driver.ping(message, callback);
}
```
- example usage
```shell
...
handshake from the client yet. In this case, calls to 'ws.send()' will buffer
the message in memory until the handshake is complete, at which point any
buffered messages will be sent to the client.

If you need to detect when the WebSocket handshake is complete, you can use the
'onopen' event.

If the connection's protocol version supports it, you can call 'ws.ping()' to
send a ping message and wait for the client's response. This method takes a
message string, and an optional callback that fires when a matching pong message
is received. It returns 'true' if and only if a ping message was sent. If the
client does not support ping/pong, this method sends no data and returns
'false'.

'''js
...
```

#### <a name="apidoc.element.faye-websocket.super_.prototype.removeEventListener"></a>[function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>removeEventListener (eventType, listener, useCapture)](#apidoc.element.faye-websocket.super_.prototype.removeEventListener)
- description and source-code
```javascript
removeEventListener = function (eventType, listener, useCapture) {
  this.removeListener(eventType, listener);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.super_.prototype.resume"></a>[function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>resume ()](#apidoc.element.faye-websocket.super_.prototype.resume)
- description and source-code
```javascript
resume = function () {
  return this._driver.messages.resume();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.faye-websocket.super_.prototype.send"></a>[function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>send (data)](#apidoc.element.faye-websocket.super_.prototype.send)
- description and source-code
```javascript
send = function (data) {
  if (this.readyState > API.OPEN) return false;
  if (!(data instanceof Buffer)) data = String(data);
  return this._driver.messages.write(data);
}
```
- example usage
```shell
...
var server = http.createServer();

server.on('upgrade', function(request, socket, body) {
if (WebSocket.isWebSocket(request)) {
  var ws = new WebSocket(request, socket, body);

  ws.on('message', function(event) {
    ws.send(event.data);
  });

  ws.on('close', function(event) {
    console.log('close', event.code, event.reason);
    ws = null;
  });
}
...
```

#### <a name="apidoc.element.faye-websocket.super_.prototype.write"></a>[function <span class="apidocSignatureSpan">faye-websocket.super_.prototype.</span>write (data)](#apidoc.element.faye-websocket.super_.prototype.write)
- description and source-code
```javascript
write = function (data) {
  return this.send(data);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
