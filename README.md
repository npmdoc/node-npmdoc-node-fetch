# api documentation for  [node-fetch (v1.6.3)](https://github.com/bitinn/node-fetch)  [![npm package](https://img.shields.io/npm/v/npmdoc-node-fetch.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-node-fetch) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-node-fetch.svg)](https://travis-ci.org/npmdoc/node-npmdoc-node-fetch)
#### A light-weight module that brings window.fetch to node.js and io.js

[![NPM](https://nodei.co/npm/node-fetch.png?downloads=true)](https://www.npmjs.com/package/node-fetch)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-fetch/build/screenCapture.buildNpmdoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-node-fetch%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-fetch/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-node-fetch/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-node-fetch/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "David Frank"
    },
    "bugs": {
        "url": "https://github.com/bitinn/node-fetch/issues"
    },
    "dependencies": {
        "encoding": "^0.1.11",
        "is-stream": "^1.0.1"
    },
    "description": "A light-weight module that brings window.fetch to node.js and io.js",
    "devDependencies": {
        "bluebird": "^3.3.4",
        "chai": "^3.5.0",
        "chai-as-promised": "^5.2.0",
        "coveralls": "^2.11.2",
        "form-data": ">=1.0.0",
        "istanbul": "^0.4.2",
        "mocha": "^2.1.0",
        "parted": "^0.1.1",
        "promise": "^7.1.1",
        "resumer": "0.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "dc234edd6489982d58e8f0db4f695029abcd8c04",
        "tarball": "https://registry.npmjs.org/node-fetch/-/node-fetch-1.6.3.tgz"
    },
    "gitHead": "3c053ce32760d2d5d6cb8712fb4115b44e4083d4",
    "homepage": "https://github.com/bitinn/node-fetch",
    "keywords": [
        "fetch",
        "http",
        "promise"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "bitinn",
            "email": "bitinn@gmail.com"
        }
    ],
    "name": "node-fetch",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/bitinn/node-fetch.git"
    },
    "scripts": {
        "coverage": "istanbul cover _mocha --report lcovonly -- -R spec test/test.js && cat ./coverage/lcov.info | coveralls",
        "report": "istanbul cover _mocha -- -R spec test/test.js",
        "test": "mocha test/test.js"
    },
    "version": "1.6.3"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module node-fetch](#apidoc.module.node-fetch)
1.  [function <span class="apidocSignatureSpan">node-fetch.</span>Headers (headers)](#apidoc.element.node-fetch.Headers)
1.  [function <span class="apidocSignatureSpan">node-fetch.</span>Promise ()](#apidoc.element.node-fetch.Promise)
1.  [function <span class="apidocSignatureSpan">node-fetch.</span>Request (input, init)](#apidoc.element.node-fetch.Request)
1.  [function <span class="apidocSignatureSpan">node-fetch.</span>Response (body, opts)](#apidoc.element.node-fetch.Response)
1.  [function <span class="apidocSignatureSpan">node-fetch.</span>body (body, opts)](#apidoc.element.node-fetch.body)
1.  [function <span class="apidocSignatureSpan">node-fetch.</span>default (url, opts)](#apidoc.element.node-fetch.default)
1.  [function <span class="apidocSignatureSpan">node-fetch.</span>fetch_error (message, type, systemError)](#apidoc.element.node-fetch.fetch_error)
1.  object <span class="apidocSignatureSpan">node-fetch.</span>Headers.prototype
1.  object <span class="apidocSignatureSpan">node-fetch.</span>Request.prototype
1.  object <span class="apidocSignatureSpan">node-fetch.</span>Response.prototype
1.  object <span class="apidocSignatureSpan">node-fetch.</span>body.prototype

#### [module node-fetch.Headers](#apidoc.module.node-fetch.Headers)
1.  [function <span class="apidocSignatureSpan">node-fetch.</span>Headers (headers)](#apidoc.element.node-fetch.Headers.Headers)

#### [module node-fetch.Headers.prototype](#apidoc.module.node-fetch.Headers.prototype)
1.  [function <span class="apidocSignatureSpan">node-fetch.Headers.prototype.</span>append (name, value)](#apidoc.element.node-fetch.Headers.prototype.append)
1.  [function <span class="apidocSignatureSpan">node-fetch.Headers.prototype.</span>delete (name)](#apidoc.element.node-fetch.Headers.prototype.delete)
1.  [function <span class="apidocSignatureSpan">node-fetch.Headers.prototype.</span>forEach (callback, thisArg)](#apidoc.element.node-fetch.Headers.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">node-fetch.Headers.prototype.</span>get (name)](#apidoc.element.node-fetch.Headers.prototype.get)
1.  [function <span class="apidocSignatureSpan">node-fetch.Headers.prototype.</span>getAll (name)](#apidoc.element.node-fetch.Headers.prototype.getAll)
1.  [function <span class="apidocSignatureSpan">node-fetch.Headers.prototype.</span>has (name)](#apidoc.element.node-fetch.Headers.prototype.has)
1.  [function <span class="apidocSignatureSpan">node-fetch.Headers.prototype.</span>raw ()](#apidoc.element.node-fetch.Headers.prototype.raw)
1.  [function <span class="apidocSignatureSpan">node-fetch.Headers.prototype.</span>set (name, value)](#apidoc.element.node-fetch.Headers.prototype.set)

#### [module node-fetch.Request](#apidoc.module.node-fetch.Request)
1.  [function <span class="apidocSignatureSpan">node-fetch.</span>Request (input, init)](#apidoc.element.node-fetch.Request.Request)

#### [module node-fetch.Request.prototype](#apidoc.module.node-fetch.Request.prototype)
1.  [function <span class="apidocSignatureSpan">node-fetch.Request.prototype.</span>clone ()](#apidoc.element.node-fetch.Request.prototype.clone)

#### [module node-fetch.Response](#apidoc.module.node-fetch.Response)
1.  [function <span class="apidocSignatureSpan">node-fetch.</span>Response (body, opts)](#apidoc.element.node-fetch.Response.Response)

#### [module node-fetch.Response.prototype](#apidoc.module.node-fetch.Response.prototype)
1.  [function <span class="apidocSignatureSpan">node-fetch.Response.prototype.</span>clone ()](#apidoc.element.node-fetch.Response.prototype.clone)

#### [module node-fetch.body](#apidoc.module.node-fetch.body)
1.  [function <span class="apidocSignatureSpan">node-fetch.</span>body (body, opts)](#apidoc.element.node-fetch.body.body)
1.  [function <span class="apidocSignatureSpan">node-fetch.body.</span>Promise ()](#apidoc.element.node-fetch.body.Promise)

#### [module node-fetch.body.prototype](#apidoc.module.node-fetch.body.prototype)
1.  [function <span class="apidocSignatureSpan">node-fetch.body.prototype.</span>_clone (instance)](#apidoc.element.node-fetch.body.prototype._clone)
1.  [function <span class="apidocSignatureSpan">node-fetch.body.prototype.</span>_convert (encoding)](#apidoc.element.node-fetch.body.prototype._convert)
1.  [function <span class="apidocSignatureSpan">node-fetch.body.prototype.</span>_decode ()](#apidoc.element.node-fetch.body.prototype._decode)
1.  [function <span class="apidocSignatureSpan">node-fetch.body.prototype.</span>buffer ()](#apidoc.element.node-fetch.body.prototype.buffer)
1.  [function <span class="apidocSignatureSpan">node-fetch.body.prototype.</span>json ()](#apidoc.element.node-fetch.body.prototype.json)
1.  [function <span class="apidocSignatureSpan">node-fetch.body.prototype.</span>text ()](#apidoc.element.node-fetch.body.prototype.text)

#### [module node-fetch.fetch_error](#apidoc.module.node-fetch.fetch_error)
1.  [function <span class="apidocSignatureSpan">node-fetch.</span>fetch_error (message, type, systemError)](#apidoc.element.node-fetch.fetch_error.fetch_error)
1.  [function <span class="apidocSignatureSpan">node-fetch.fetch_error.</span>super_ ()](#apidoc.element.node-fetch.fetch_error.super_)



# <a name="apidoc.module.node-fetch"></a>[module node-fetch](#apidoc.module.node-fetch)

#### <a name="apidoc.element.node-fetch.Headers"></a>[function <span class="apidocSignatureSpan">node-fetch.</span>Headers (headers)](#apidoc.element.node-fetch.Headers)
- description and source-code
```javascript
function Headers(headers) {

	var self = this;
	this._headers = {};

	// Headers
	if (headers instanceof Headers) {
		headers = headers.raw();
	}

	// plain object
	for (var prop in headers) {
		if (!headers.hasOwnProperty(prop)) {
			continue;
		}

		if (typeof headers[prop] === 'string') {
			this.set(prop, headers[prop]);

		} else if (typeof headers[prop] === 'number' && !isNaN(headers[prop])) {
			this.set(prop, headers[prop].toString());

		} else if (headers[prop] instanceof Array) {
			headers[prop].forEach(function(item) {
				self.append(prop, item.toString());
			});
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-fetch.Promise"></a>[function <span class="apidocSignatureSpan">node-fetch.</span>Promise ()](#apidoc.element.node-fetch.Promise)
- description and source-code
```javascript
function Promise() { [native code] }
```
- example usage
```shell
...
	}

	Body.Promise = Fetch.Promise;

	var self = this;

	// wrap http.request into fetch
	return new Fetch.Promise(function(resolve, reject) {
		// build request object
		var options = new Request(url, opts);

		if (!options.protocol || !options.hostname) {
			throw new Error('only absolute urls are supported');
		}
...
```

#### <a name="apidoc.element.node-fetch.Request"></a>[function <span class="apidocSignatureSpan">node-fetch.</span>Request (input, init)](#apidoc.element.node-fetch.Request)
- description and source-code
```javascript
function Request(input, init) {
	var url, url_parsed;

	// normalize input
	if (!(input instanceof Request)) {
		url = input;
		url_parsed = parse_url(url);
		input = {};
	} else {
		url = input.url;
		url_parsed = parse_url(url);
	}

	// normalize init
	init = init || {};

	// fetch spec options
	this.method = init.method || input.method || 'GET';
	this.redirect = init.redirect || input.redirect || 'follow';
	this.headers = new Headers(init.headers || input.headers || {});
	this.url = url;

	// server only options
	this.follow = init.follow !== undefined ?
		init.follow : input.follow !== undefined ?
		input.follow : 20;
	this.compress = init.compress !== undefined ?
		init.compress : input.compress !== undefined ?
		input.compress : true;
	this.counter = init.counter || input.counter || 0;
	this.agent = init.agent || input.agent;

	Body.call(this, init.body || this._clone(input), {
		timeout: init.timeout || input.timeout || 0,
		size: init.size || input.size || 0
	});

	// server request options
	this.protocol = url_parsed.protocol;
	this.hostname = url_parsed.hostname;
	this.port = url_parsed.port;
	this.path = url_parsed.path;
	this.auth = url_parsed.auth;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-fetch.Response"></a>[function <span class="apidocSignatureSpan">node-fetch.</span>Response (body, opts)](#apidoc.element.node-fetch.Response)
- description and source-code
```javascript
function Response(body, opts) {

	opts = opts || {};

	this.url = opts.url;
	this.status = opts.status || 200;
	this.statusText = opts.statusText || http.STATUS_CODES[this.status];
	this.headers = new Headers(opts.headers);
	this.ok = this.status >= 200 && this.status < 300;

	Body.call(this, body, opts);

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-fetch.body"></a>[function <span class="apidocSignatureSpan">node-fetch.</span>body (body, opts)](#apidoc.element.node-fetch.body)
- description and source-code
```javascript
function Body(body, opts) {

	opts = opts || {};

	this.body = body;
	this.bodyUsed = false;
	this.size = opts.size || 0;
	this.timeout = opts.timeout || 0;
	this._raw = [];
	this._abort = false;

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-fetch.default"></a>[function <span class="apidocSignatureSpan">node-fetch.</span>default (url, opts)](#apidoc.element.node-fetch.default)
- description and source-code
```javascript
function Fetch(url, opts) {

	// allow call as function
	if (!(this instanceof Fetch))
		return new Fetch(url, opts);

	// allow custom promise
	if (!Fetch.Promise) {
		throw new Error('native promise missing, set Fetch.Promise to your favorite alternative');
	}

	Body.Promise = Fetch.Promise;

	var self = this;

	// wrap http.request into fetch
	return new Fetch.Promise(function(resolve, reject) {
		// build request object
		var options = new Request(url, opts);

		if (!options.protocol || !options.hostname) {
			throw new Error('only absolute urls are supported');
		}

		if (options.protocol !== 'http:' && options.protocol !== 'https:') {
			throw new Error('only http(s) protocols are supported');
		}

		var send;
		if (options.protocol === 'https:') {
			send = https.request;
		} else {
			send = http.request;
		}

		// normalize headers
		var headers = new Headers(options.headers);

		if (options.compress) {
			headers.set('accept-encoding', 'gzip,deflate');
		}

		if (!headers.has('user-agent')) {
			headers.set('user-agent', 'node-fetch/1.0 (+https://github.com/bitinn/node-fetch)');
		}

		if (!headers.has('connection') && !options.agent) {
			headers.set('connection', 'close');
		}

		if (!headers.has('accept')) {
			headers.set('accept', '*/*');
		}

		// detect form data input from form-data module, this hack avoid the need to pass multipart header manually
		if (!headers.has('content-type') && options.body && typeof options.body.getBoundary === 'function') {
			headers.set('content-type', 'multipart/form-data; boundary=' + options.body.getBoundary());
		}

		// bring node-fetch closer to browser behavior by setting content-length automatically
		if (!headers.has('content-length') && /post|put|patch|delete/i.test(options.method)) {
			if (typeof options.body === 'string') {
				headers.set('content-length', Buffer.byteLength(options.body));
			// detect form data input from form-data module, this hack avoid the need to add content-length header manually
			} else if (options.body && typeof options.body.getLengthSync === 'function') {
				// for form-data 1.x
				if (options.body._lengthRetrievers && options.body._lengthRetrievers.length == 0) {
					headers.set('content-length', options.body.getLengthSync().toString());
				// for form-data 2.x
				} else if (options.body.hasKnownLength && options.body.hasKnownLength()) {
					headers.set('content-length', options.body.getLengthSync().toString());
				}
			// this is only necessary for older nodejs releases (before iojs merge)
			} else if (options.body === undefined || options.body === null) {
				headers.set('content-length', '0');
			}
		}

		options.headers = headers.raw();

		// http.request only support string as host header, this hack make custom host header possible
		if (options.headers.host) {
			options.headers.host = options.headers.host[0];
		}

		// send request
		var req = send(options);
		var reqTimeout;

		if (options.timeout) {
			req.once('socket', function(socket) {
				reqTimeout = setTimeout(function() {
					req.abort();
					reject(new FetchError('network timeout at: ' + options.url, 'request-timeout'));
				}, options.timeout);
			});
		}

		req.on('error', function(err) {
			clearTimeout(reqTimeout);
			reject(new FetchError('request to ' + options.url + ' failed, reason: ' + err.message, 'system', err));
		});

		req.on('response', function(res) {
			clearTimeout(reqTimeout);

			// handle redirect
			if (self.isRedirect(res.statusCode) && options.redirect !== 'manual') {
				if (options.redirect === 'error') {
					reject(new FetchError('redirect mode is set to error: ' + options.url, 'no-redirect'));
					return;
				}

				if (options.counter >= options.follow) {
					reject(new FetchError('maximum redirect reached at: ' + options.url, 'max-redirect'));
					return;
				}

				if (!res.headers.location) {
					reject(new FetchError('redirect location header missing at: ' + options.url, 'invalid-redirect'));
					return;
				}

				// per fetch spec, for POST request with 301/302 response, or any request with 303 response, use GET wh ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-fetch.fetch_error"></a>[function <span class="apidocSignatureSpan">node-fetch.</span>fetch_error (message, type, systemError)](#apidoc.element.node-fetch.fetch_error)
- description and source-code
```javascript
function FetchError(message, type, systemError) {

	// hide custom error implementation details from end-users
	Error.captureStackTrace(this, this.constructor);

	this.name = this.constructor.name;
	this.message = message;
	this.type = type;

	// when err.type is 'system', err.code contains system error code
	if (systemError) {
		this.code = this.errno = systemError.code;
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-fetch.Headers"></a>[module node-fetch.Headers](#apidoc.module.node-fetch.Headers)

#### <a name="apidoc.element.node-fetch.Headers.Headers"></a>[function <span class="apidocSignatureSpan">node-fetch.</span>Headers (headers)](#apidoc.element.node-fetch.Headers.Headers)
- description and source-code
```javascript
function Headers(headers) {

	var self = this;
	this._headers = {};

	// Headers
	if (headers instanceof Headers) {
		headers = headers.raw();
	}

	// plain object
	for (var prop in headers) {
		if (!headers.hasOwnProperty(prop)) {
			continue;
		}

		if (typeof headers[prop] === 'string') {
			this.set(prop, headers[prop]);

		} else if (typeof headers[prop] === 'number' && !isNaN(headers[prop])) {
			this.set(prop, headers[prop].toString());

		} else if (headers[prop] instanceof Array) {
			headers[prop].forEach(function(item) {
				self.append(prop, item.toString());
			});
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-fetch.Headers.prototype"></a>[module node-fetch.Headers.prototype](#apidoc.module.node-fetch.Headers.prototype)

#### <a name="apidoc.element.node-fetch.Headers.prototype.append"></a>[function <span class="apidocSignatureSpan">node-fetch.Headers.prototype.</span>append (name, value)](#apidoc.element.node-fetch.Headers.prototype.append)
- description and source-code
```javascript
append = function (name, value) {
	if (!this.has(name)) {
		this.set(name, value);
		return;
	}

	this._headers[name.toLowerCase()].push(value);
}
```
- example usage
```shell
...
		console.log(json);
	});

// post with form-data (detect multipart)

var FormData = require('form-data');
var form = new FormData();
form.append('a', 1);
fetch('http://httpbin.org/post', { method: 'POST', body: form })
	.then(function(res) {
		return res.json();
	}).then(function(json) {
		console.log(json);
	});
...
```

#### <a name="apidoc.element.node-fetch.Headers.prototype.delete"></a>[function <span class="apidocSignatureSpan">node-fetch.Headers.prototype.</span>delete (name)](#apidoc.element.node-fetch.Headers.prototype.delete)
- description and source-code
```javascript
delete = function (name) {
	delete this._headers[name.toLowerCase()];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-fetch.Headers.prototype.forEach"></a>[function <span class="apidocSignatureSpan">node-fetch.Headers.prototype.</span>forEach (callback, thisArg)](#apidoc.element.node-fetch.Headers.prototype.forEach)
- description and source-code
```javascript
forEach = function (callback, thisArg) {
	Object.getOwnPropertyNames(this._headers).forEach(function(name) {
		this._headers[name].forEach(function(value) {
			callback.call(thisArg, value, name, this)
		}, this)
	}, this)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-fetch.Headers.prototype.get"></a>[function <span class="apidocSignatureSpan">node-fetch.Headers.prototype.</span>get (name)](#apidoc.element.node-fetch.Headers.prototype.get)
- description and source-code
```javascript
get = function (name) {
	var list = this._headers[name.toLowerCase()];
	return list ? list[0] : null;
}
```
- example usage
```shell
...

fetch('https://github.com/')
	.then(function(res) {
		console.log(res.ok);
		console.log(res.status);
		console.log(res.statusText);
		console.log(res.headers.raw());
		console.log(res.headers.get('content-type'));
	});

// post

fetch('http://httpbin.org/post', { method: 'POST', body: 'a=1' })
	.then(function(res) {
		return res.json();
...
```

#### <a name="apidoc.element.node-fetch.Headers.prototype.getAll"></a>[function <span class="apidocSignatureSpan">node-fetch.Headers.prototype.</span>getAll (name)](#apidoc.element.node-fetch.Headers.prototype.getAll)
- description and source-code
```javascript
getAll = function (name) {
	if (!this.has(name)) {
		return [];
	}

	return this._headers[name.toLowerCase()];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-fetch.Headers.prototype.has"></a>[function <span class="apidocSignatureSpan">node-fetch.Headers.prototype.</span>has (name)](#apidoc.element.node-fetch.Headers.prototype.has)
- description and source-code
```javascript
has = function (name) {
	return this._headers.hasOwnProperty(name.toLowerCase());
}
```
- example usage
```shell
...
		// normalize headers
		var headers = new Headers(options.headers);

		if (options.compress) {
			headers.set('accept-encoding', 'gzip,deflate');
		}

		if (!headers.has('user-agent')) {
			headers.set('user-agent', 'node-fetch/1.0 (+https://github.com/bitinn/node-fetch)');
		}

		if (!headers.has('connection') && !options.agent) {
			headers.set('connection', 'close');
		}
...
```

#### <a name="apidoc.element.node-fetch.Headers.prototype.raw"></a>[function <span class="apidocSignatureSpan">node-fetch.Headers.prototype.</span>raw ()](#apidoc.element.node-fetch.Headers.prototype.raw)
- description and source-code
```javascript
raw = function () {
	return this._headers;
}
```
- example usage
```shell
...
// meta

fetch('https://github.com/')
	.then(function(res) {
		console.log(res.ok);
		console.log(res.status);
		console.log(res.statusText);
		console.log(res.headers.raw());
		console.log(res.headers.get('content-type'));
	});

// post

fetch('http://httpbin.org/post', { method: 'POST', body: 'a=1' })
	.then(function(res) {
...
```

#### <a name="apidoc.element.node-fetch.Headers.prototype.set"></a>[function <span class="apidocSignatureSpan">node-fetch.Headers.prototype.</span>set (name, value)](#apidoc.element.node-fetch.Headers.prototype.set)
- description and source-code
```javascript
set = function (name, value) {
	this._headers[name.toLowerCase()] = [value];
}
```
- example usage
```shell
...
			send = http.request;
		}

		// normalize headers
		var headers = new Headers(options.headers);

		if (options.compress) {
			headers.set('accept-encoding', 'gzip,deflate');
		}

		if (!headers.has('user-agent')) {
			headers.set('user-agent', 'node-fetch/1.0 (+https://github.com/bitinn/node-fetch)');
		}

		if (!headers.has('connection') && !options.agent) {
...
```



# <a name="apidoc.module.node-fetch.Request"></a>[module node-fetch.Request](#apidoc.module.node-fetch.Request)

#### <a name="apidoc.element.node-fetch.Request.Request"></a>[function <span class="apidocSignatureSpan">node-fetch.</span>Request (input, init)](#apidoc.element.node-fetch.Request.Request)
- description and source-code
```javascript
function Request(input, init) {
	var url, url_parsed;

	// normalize input
	if (!(input instanceof Request)) {
		url = input;
		url_parsed = parse_url(url);
		input = {};
	} else {
		url = input.url;
		url_parsed = parse_url(url);
	}

	// normalize init
	init = init || {};

	// fetch spec options
	this.method = init.method || input.method || 'GET';
	this.redirect = init.redirect || input.redirect || 'follow';
	this.headers = new Headers(init.headers || input.headers || {});
	this.url = url;

	// server only options
	this.follow = init.follow !== undefined ?
		init.follow : input.follow !== undefined ?
		input.follow : 20;
	this.compress = init.compress !== undefined ?
		init.compress : input.compress !== undefined ?
		input.compress : true;
	this.counter = init.counter || input.counter || 0;
	this.agent = init.agent || input.agent;

	Body.call(this, init.body || this._clone(input), {
		timeout: init.timeout || input.timeout || 0,
		size: init.size || input.size || 0
	});

	// server request options
	this.protocol = url_parsed.protocol;
	this.hostname = url_parsed.hostname;
	this.port = url_parsed.port;
	this.path = url_parsed.path;
	this.auth = url_parsed.auth;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-fetch.Request.prototype"></a>[module node-fetch.Request.prototype](#apidoc.module.node-fetch.Request.prototype)

#### <a name="apidoc.element.node-fetch.Request.prototype.clone"></a>[function <span class="apidocSignatureSpan">node-fetch.Request.prototype.</span>clone ()](#apidoc.element.node-fetch.Request.prototype.clone)
- description and source-code
```javascript
clone = function () {
	return new Request(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-fetch.Response"></a>[module node-fetch.Response](#apidoc.module.node-fetch.Response)

#### <a name="apidoc.element.node-fetch.Response.Response"></a>[function <span class="apidocSignatureSpan">node-fetch.</span>Response (body, opts)](#apidoc.element.node-fetch.Response.Response)
- description and source-code
```javascript
function Response(body, opts) {

	opts = opts || {};

	this.url = opts.url;
	this.status = opts.status || 200;
	this.statusText = opts.statusText || http.STATUS_CODES[this.status];
	this.headers = new Headers(opts.headers);
	this.ok = this.status >= 200 && this.status < 300;

	Body.call(this, body, opts);

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-fetch.Response.prototype"></a>[module node-fetch.Response.prototype](#apidoc.module.node-fetch.Response.prototype)

#### <a name="apidoc.element.node-fetch.Response.prototype.clone"></a>[function <span class="apidocSignatureSpan">node-fetch.Response.prototype.</span>clone ()](#apidoc.element.node-fetch.Response.prototype.clone)
- description and source-code
```javascript
clone = function () {
	return new Response(this._clone(this), {
		url: this.url
		, status: this.status
		, statusText: this.statusText
		, headers: this.headers
		, ok: this.ok
	});
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-fetch.body"></a>[module node-fetch.body](#apidoc.module.node-fetch.body)

#### <a name="apidoc.element.node-fetch.body.body"></a>[function <span class="apidocSignatureSpan">node-fetch.</span>body (body, opts)](#apidoc.element.node-fetch.body.body)
- description and source-code
```javascript
function Body(body, opts) {

	opts = opts || {};

	this.body = body;
	this.bodyUsed = false;
	this.size = opts.size || 0;
	this.timeout = opts.timeout || 0;
	this._raw = [];
	this._abort = false;

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-fetch.body.Promise"></a>[function <span class="apidocSignatureSpan">node-fetch.body.</span>Promise ()](#apidoc.element.node-fetch.body.Promise)
- description and source-code
```javascript
function Promise() { [native code] }
```
- example usage
```shell
...
	}

	Body.Promise = Fetch.Promise;

	var self = this;

	// wrap http.request into fetch
	return new Fetch.Promise(function(resolve, reject) {
		// build request object
		var options = new Request(url, opts);

		if (!options.protocol || !options.hostname) {
			throw new Error('only absolute urls are supported');
		}
...
```



# <a name="apidoc.module.node-fetch.body.prototype"></a>[module node-fetch.body.prototype](#apidoc.module.node-fetch.body.prototype)

#### <a name="apidoc.element.node-fetch.body.prototype._clone"></a>[function <span class="apidocSignatureSpan">node-fetch.body.prototype.</span>_clone (instance)](#apidoc.element.node-fetch.body.prototype._clone)
- description and source-code
```javascript
_clone = function (instance) {
	var p1, p2;
	var body = instance.body;

	// don't allow cloning a used body
	if (instance.bodyUsed) {
		throw new Error('cannot clone body after it is used');
	}

	// check that body is a stream and not form-data object
	// note: we can't clone the form-data object without having it as a dependency
	if (bodyStream(body) && typeof body.getBoundary !== 'function') {
		// tee instance body
		p1 = new PassThrough();
		p2 = new PassThrough();
		body.pipe(p1);
		body.pipe(p2);
		// set instance body to teed body and return the other teed body
		instance.body = p1;
		body = p2;
	}

	return body;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-fetch.body.prototype._convert"></a>[function <span class="apidocSignatureSpan">node-fetch.body.prototype.</span>_convert (encoding)](#apidoc.element.node-fetch.body.prototype._convert)
- description and source-code
```javascript
_convert = function (encoding) {

	encoding = encoding || 'utf-8';

	var ct = this.headers.get('content-type');
	var charset = 'utf-8';
	var res, str;

	// header
	if (ct) {
		// skip encoding detection altogether if not html/xml/plain text
		if (!/text\/html|text\/plain|\+xml|\/xml/i.test(ct)) {
			return Buffer.concat(this._raw);
		}

		res = /charset=([^;]*)/i.exec(ct);
	}

	// no charset in content type, peek at response body for at most 1024 bytes
	if (!res && this._raw.length > 0) {
		for (var i = 0; i < this._raw.length; i++) {
			str += this._raw[i].toString()
			if (str.length > 1024) {
				break;
			}
		}
		str = str.substr(0, 1024);
	}

	// html5
	if (!res && str) {
		res = /<meta.+?charset=(['"])(.+?)\1/i.exec(str);
	}

	// html4
	if (!res && str) {
		res = /<meta[\s]+?http-equiv=(['"])content-type\1[\s]+?content=(['"])(.+?)\2/i.exec(str);

		if (res) {
			res = /charset=(.*)/i.exec(res.pop());
		}
	}

	// xml
	if (!res && str) {
		res = /<\?xml.+?encoding=(['"])(.+?)\1/i.exec(str);
	}

	// found charset
	if (res) {
		charset = res.pop();

		// prevent decode issues when sites use incorrect encoding
		// ref: https://hsivonen.fi/encoding-menu/
		if (charset === 'gb2312' || charset === 'gbk') {
			charset = 'gb18030';
		}
	}

	// turn raw buffers into a single utf-8 buffer
	return convert(
		Buffer.concat(this._raw)
		, encoding
		, charset
	);

}
```
- example usage
```shell
...
	return new Body.Promise(function(resolve, reject) {
		var resTimeout;

		// body is string
		if (typeof self.body === 'string') {
			self._bytes = self.body.length;
			self._raw = [new Buffer(self.body)];
			return resolve(self._convert());
		}

		// body is buffer
		if (self.body instanceof Buffer) {
			self._bytes = self.body.length;
			self._raw = [self.body];
			return resolve(self._convert());
...
```

#### <a name="apidoc.element.node-fetch.body.prototype._decode"></a>[function <span class="apidocSignatureSpan">node-fetch.body.prototype.</span>_decode ()](#apidoc.element.node-fetch.body.prototype._decode)
- description and source-code
```javascript
_decode = function () {

	var self = this;

	if (this.bodyUsed) {
		return Body.Promise.reject(new Error('body used already for: ' + this.url));
	}

	this.bodyUsed = true;
	this._bytes = 0;
	this._abort = false;
	this._raw = [];

	return new Body.Promise(function(resolve, reject) {
		var resTimeout;

		// body is string
		if (typeof self.body === 'string') {
			self._bytes = self.body.length;
			self._raw = [new Buffer(self.body)];
			return resolve(self._convert());
		}

		// body is buffer
		if (self.body instanceof Buffer) {
			self._bytes = self.body.length;
			self._raw = [self.body];
			return resolve(self._convert());
		}

		// allow timeout on slow response body
		if (self.timeout) {
			resTimeout = setTimeout(function() {
				self._abort = true;
				reject(new FetchError('response timeout at ' + self.url + ' over limit: ' + self.timeout, 'body-timeout'));
			}, self.timeout);
		}

		// handle stream error, such as incorrect content-encoding
		self.body.on('error', function(err) {
			reject(new FetchError('invalid response body at: ' + self.url + ' reason: ' + err.message, 'system', err));
		});

		// body is stream
		self.body.on('data', function(chunk) {
			if (self._abort || chunk === null) {
				return;
			}

			if (self.size && self._bytes + chunk.length > self.size) {
				self._abort = true;
				reject(new FetchError('content size at ' + self.url + ' over limit: ' + self.size, 'max-size'));
				return;
			}

			self._bytes += chunk.length;
			self._raw.push(chunk);
		});

		self.body.on('end', function() {
			if (self._abort) {
				return;
			}

			clearTimeout(resTimeout);
			resolve(self._convert());
		});
	});

}
```
- example usage
```shell
...
Body.prototype.json = function() {

	// for 204 No Content response, buffer will be empty, parsing it will throw error
	if (this.status === 204) {
		return Body.Promise.resolve({});
	}

	return this._decode().then(function(buffer) {
		return JSON.parse(buffer.toString());
	});

};

/**
* Decode response as text
...
```

#### <a name="apidoc.element.node-fetch.body.prototype.buffer"></a>[function <span class="apidocSignatureSpan">node-fetch.body.prototype.</span>buffer ()](#apidoc.element.node-fetch.body.prototype.buffer)
- description and source-code
```javascript
buffer = function () {

	return this._decode();

}
```
- example usage
```shell
...
// buffer
// if you prefer to cache binary data in full, use buffer()
// note that buffer() is a node-fetch only API

var fileType = require('file-type');
fetch('https://assets-cdn.github.com/images/modules/logos_page/Octocat.png')
	.then(function(res) {
		return res.buffer();
	}).then(function(buffer) {
		fileType(buffer);
	});

// meta

fetch('https://github.com/')
...
```

#### <a name="apidoc.element.node-fetch.body.prototype.json"></a>[function <span class="apidocSignatureSpan">node-fetch.body.prototype.</span>json ()](#apidoc.element.node-fetch.body.prototype.json)
- description and source-code
```javascript
json = function () {

	// for 204 No Content response, buffer will be empty, parsing it will throw error
	if (this.status === 204) {
		return Body.Promise.resolve({});
	}

	return this._decode().then(function(buffer) {
		return JSON.parse(buffer.toString());
	});

}
```
- example usage
```shell
...

# Features

- Stay consistent with 'window.fetch' API.
- Make conscious trade-off when following [whatwg fetch spec](https://fetch.spec.whatwg.org/) and [stream spec](https://streams.
spec.whatwg.org/) implementation details, document known difference.
- Use native promise, but allow substituting it with [insert your favorite promise library].
- Use native stream for body, on both request and response.
- Decode content encoding (gzip/deflate) properly, and convert string output (such as 'res.text()' and 'res.json()') to UTF-8 automatically
.
- Useful extensions such as timeout, redirect limit, response size limit, [explicit errors](https://github.com/bitinn/node-fetch
/blob/master/ERROR-HANDLING.md) for troubleshooting.


# Difference from client-side fetch

- See [Known Differences](https://github.com/bitinn/node-fetch/blob/master/LIMITS.md) for details.
- If you happen to use a missing feature that 'window.fetch' offers, feel free to open an issue.
...
```

#### <a name="apidoc.element.node-fetch.body.prototype.text"></a>[function <span class="apidocSignatureSpan">node-fetch.body.prototype.</span>text ()](#apidoc.element.node-fetch.body.prototype.text)
- description and source-code
```javascript
text = function () {

	return this._decode().then(function(buffer) {
		return buffer.toString();
	});

}
```
- example usage
```shell
...

# Features

- Stay consistent with 'window.fetch' API.
- Make conscious trade-off when following [whatwg fetch spec](https://fetch.spec.whatwg.org/) and [stream spec](https://streams.
spec.whatwg.org/) implementation details, document known difference.
- Use native promise, but allow substituting it with [insert your favorite promise library].
- Use native stream for body, on both request and response.
- Decode content encoding (gzip/deflate) properly, and convert string output (such as 'res.text()' and 'res.json()') to UTF-8 automatically
.
- Useful extensions such as timeout, redirect limit, response size limit, [explicit errors](https://github.com/bitinn/node-fetch
/blob/master/ERROR-HANDLING.md) for troubleshooting.


# Difference from client-side fetch

- See [Known Differences](https://github.com/bitinn/node-fetch/blob/master/LIMITS.md) for details.
- If you happen to use a missing feature that 'window.fetch' offers, feel free to open an issue.
...
```



# <a name="apidoc.module.node-fetch.fetch_error"></a>[module node-fetch.fetch_error](#apidoc.module.node-fetch.fetch_error)

#### <a name="apidoc.element.node-fetch.fetch_error.fetch_error"></a>[function <span class="apidocSignatureSpan">node-fetch.</span>fetch_error (message, type, systemError)](#apidoc.element.node-fetch.fetch_error.fetch_error)
- description and source-code
```javascript
function FetchError(message, type, systemError) {

	// hide custom error implementation details from end-users
	Error.captureStackTrace(this, this.constructor);

	this.name = this.constructor.name;
	this.message = message;
	this.type = type;

	// when err.type is 'system', err.code contains system error code
	if (systemError) {
		this.code = this.errno = systemError.code;
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-fetch.fetch_error.super_"></a>[function <span class="apidocSignatureSpan">node-fetch.fetch_error.</span>super_ ()](#apidoc.element.node-fetch.fetch_error.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
