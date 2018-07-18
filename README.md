<h1 align="center">🎾 Koa Core</h1>

<p align="center">
  <i>
    The <b>core</b> that powers uSwitch Koa services.
  </i>
</p>

<p align="center">
  <b><a href="#overview">Overview</a></b>
  |
  <b><a href="#packages">Packages</a></b>
  |
  <b><a href="#library">Library</a></b>
  |
  <b><a href="#example">Example</a></b>
</p>

[![License](https://img.shields.io/github/license/mashape/apistatus.svg?style=for-the-badge)]()
![type](https://img.shields.io/badge/⚡-library-c45366.svg?style=for-the-badge)
![language](https://img.shields.io/badge/❤-Node-da776c.svg?style=for-the-badge)
[![test](https://img.shields.io/badge/🔬-Jest-e9a279.svg?style=for-the-badge)](https://facebook.github.io/jest/)
[![style](https://img.shields.io/badge/🎨-Standard-e4ca93.svg?style=for-the-badge)](https://standardjs.com)

## Overview

**Koa Core** is a [`lerna`](https://github.com/lerna/lerna) monorepo
housing all of **uSwitch**'s `koa` packages.

This repo acts both as a **helper** library for wiring together the
[`@uswitch/koa-`]() packages as well as a master **list** of open sources
`koa` libraries that we depend on.

This means we have a **single point of truth** for which packages we use
and the versions we depend on.

```
npm install @uswitch/koa-core
```

### Making changes

All of our `koa` libraries can be found in
[`packages`](https:/github.com/uswitch/koa-core/tree/master/packages). Any
changes should be made to them individually. Commits should ideally be
namespaced to the package you're changing.

_e.g._ `[access] Making changes to koa acceess` or `[core] Making
changes to core.`

Once changes have been committed, we use `lerna` to manage the bumping
and publishing.

```sh
npm run publish:packages
```

This will publish the individual libraries followed by performing
updating dependencies and generating the documentation for `core` .

## Packages

#### `@uswitch` packages

<!-- DO NOT REMOVE - This is generated documentation  -->
<!-- [doc-list-packages-internal:start] -->
<!-- Generated Wed Jul 18 2018 17:32:50 GMT+0100 (BST) -->
| Package | Version | Dependencies | Description |
|--|--|--|--|
| [`@uswitch/koa-access`](https://www.npmjs.com/package/@uswitch/koa-access) | [![npm](https://img.shields.io/npm/v/@uswitch/koa-access.svg?maxAge=2592000)](https://www.npmjs.com/package/@uswitch/koa-access) | [![Dependency Status](https://david-dm.org/@uswitch/koa-access.svg?path=packages/@uswitch/koa-access)](https://david-dm.org/@uswitch/koa-access?path=packages/@uswitch/koa-access) | 👌 A Koa middleware for logging JSON access logs consistently, similar to morgan |
| [`@uswitch/koa-prometheus`](https://www.npmjs.com/package/@uswitch/koa-prometheus) | [![npm](https://img.shields.io/npm/v/@uswitch/koa-prometheus.svg?maxAge=2592000)](https://www.npmjs.com/package/@uswitch/koa-prometheus) | [![Dependency Status](https://david-dm.org/@uswitch/koa-prometheus.svg?path=packages/@uswitch/koa-prometheus)](https://david-dm.org/@uswitch/koa-prometheus?path=packages/@uswitch/koa-prometheus) | 🌡️ A configurable Prometheus data collector with Koa middleware |
| [`@uswitch/koa-signal`](https://www.npmjs.com/package/@uswitch/koa-signal) | [![npm](https://img.shields.io/npm/v/@uswitch/koa-signal.svg?maxAge=2592000)](https://www.npmjs.com/package/@uswitch/koa-signal) | [![Dependency Status](https://david-dm.org/@uswitch/koa-signal.svg?path=packages/@uswitch/koa-signal)](https://david-dm.org/@uswitch/koa-signal?path=packages/@uswitch/koa-signal) | 🚦 Hackable and configurable output rendering for loggers |
| [`@uswitch/koa-timeout`](https://www.npmjs.com/package/@uswitch/koa-timeout) | [![npm](https://img.shields.io/npm/v/@uswitch/koa-timeout.svg?maxAge=2592000)](https://www.npmjs.com/package/@uswitch/koa-timeout) | [![Dependency Status](https://david-dm.org/@uswitch/koa-timeout.svg?path=packages/@uswitch/koa-timeout)](https://david-dm.org/@uswitch/koa-timeout?path=packages/@uswitch/koa-timeout) | ⏰ A Koa middleware to handle timeouts correctly |
| [`@uswitch/koa-tracer`](https://www.npmjs.com/package/@uswitch/koa-tracer) | [![npm](https://img.shields.io/npm/v/@uswitch/koa-tracer.svg?maxAge=2592000)](https://www.npmjs.com/package/@uswitch/koa-tracer) | [![Dependency Status](https://david-dm.org/@uswitch/koa-tracer.svg?path=packages/@uswitch/koa-tracer)](https://david-dm.org/@uswitch/koa-tracer?path=packages/@uswitch/koa-tracer) | 🕵️‍♀️ A koa.js middleware to add namespaced tracing throughout a requests lifecycle |
<!-- [doc-list-packages-internal:end] -->
<!-- DO NOT REMOVE - This is generated documentation -->


#### `koa` packages
<!-- DO NOT REMOVE - This is generated documentation  -->
<!-- [doc-list-packages:start] -->
<!-- Generated Wed Jul 18 2018 17:32:49 GMT+0100 (BST) -->
| Package | Version | Latest |
|--|--|--|
| [`koa`](https://www.npmjs.com/package/koa) | `^2.5.2` | [![npm](https://img.shields.io/npm/v/koa.svg?maxAge=2592000)](https://www.npmjs.com/package/koa) |
| [`koa-bodyparser`](https://www.npmjs.com/package/koa-bodyparser) | `^4.2.1` | [![npm](https://img.shields.io/npm/v/koa-bodyparser.svg?maxAge=2592000)](https://www.npmjs.com/package/koa-bodyparser) |
| [`koa-compose`](https://www.npmjs.com/package/koa-compose) | `^4.1.0` | [![npm](https://img.shields.io/npm/v/koa-compose.svg?maxAge=2592000)](https://www.npmjs.com/package/koa-compose) |
| [`koa-cookie`](https://www.npmjs.com/package/koa-cookie) | `^1.0.0` | [![npm](https://img.shields.io/npm/v/koa-cookie.svg?maxAge=2592000)](https://www.npmjs.com/package/koa-cookie) |
| [`koa-helmet`](https://www.npmjs.com/package/koa-helmet) | `^4.0.0` | [![npm](https://img.shields.io/npm/v/koa-helmet.svg?maxAge=2592000)](https://www.npmjs.com/package/koa-helmet) |
| [`koa-requestid`](https://www.npmjs.com/package/koa-requestid) | `^2.0.1` | [![npm](https://img.shields.io/npm/v/koa-requestid.svg?maxAge=2592000)](https://www.npmjs.com/package/koa-requestid) |
| [`koa-router`](https://www.npmjs.com/package/koa-router) | `^7.4.0` | [![npm](https://img.shields.io/npm/v/koa-router.svg?maxAge=2592000)](https://www.npmjs.com/package/koa-router) |
| [`koa-static`](https://www.npmjs.com/package/koa-static) | `^5.0.0` | [![npm](https://img.shields.io/npm/v/koa-static.svg?maxAge=2592000)](https://www.npmjs.com/package/koa-static) |
<!-- [doc-list-packages:end] -->
<!-- DO NOT REMOVE - This is generated documentation -->

## Library

`koa-core` can also be used as a **boilerplate** library to quickly
set upo a new **Koa** server in the same was as the [**Koa**
library](https://github.com/koajs/koa) itself.

### Usage

```js
import Koa from '@uswitch/koa-core'

const { app, logger } = new Koa()
app.listen(3000, () => logger.info('Applications started on port 3000'))
```

<p align="center"><i><b>N.B.</b> <code>koa-core</code> returns an <code>app</code> and a <code>logger</code></i></p>


### Importing dependencies

All of the [`koa` **packages**](#packages) we have are available to import in your
project via the following;

```js
/* ES6 Import */
import koaLibrary from '@uswitch/koa-core/koa-library'

/* Require */
const koaLibrary = require('@uswitch/koa-core/koa-library')
```

See [**packages**](#packages) for a list of available `koa` libraries
through `koa-core`.


## Example

This project also comes with an [**Example
server**](https://github.com/uswitch/koa-core/blob/master/__example__/server.js)
and some example
[**routes**](https://github.com/uswitch/koa-core/blob/master/__example__/server-routes.js)
which shows how we use the `@uswitch/koa` libraries.

```sh
npm install
NODE_ENV=development npm run example
NODE_ENV=production npm run example
```

This will start the server on port `http://localhost:3000` and you can
try hitting the following routes to see how it works;

```sh
curl http://localhost:3000/hello         // 200 string body
curl http://localhost:3000/hello/world

// Test different status codes
curl http://localhost:3000/status/200
curl http://localhost:3000/status/404
curl http://localhost:3000/status/503

// Test tracing errors as they happen
curl http://localhost:3000/error         // Fatal error
curl http://localhost:3000/multi-errors  // Multiple errors non fatal

// Test tracing behaviour
curl http://localhost:3000/trace/150     // Trace either side of 150ms async
curl http://localhost:3000/scope/name    // Trace message to scope NAME

// See all types of koa-signal message
curl http://localhost:3000/signal/all
```
