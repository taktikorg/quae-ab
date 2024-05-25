# String.prototype.padStart <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![dependency status][deps-svg]][deps-url]
[![dev dependency status][dev-deps-svg]][dev-deps-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

An ES2017 spec-compliant `String.prototype.padStart` shim. Invoke its "shim" method to shim `String.prototype.padStart` if it is unavailable.

This package implements the [es-shim API](https://github.com/es-shims/api) interface. It works in an ES3-supported environment and complies with the [spec](https://github.com/tc39/ecma262/pull/581).

Most common usage:
```js
var padStart = require('@taktikorg/quae-ab');

assert(padStart('foo', 5, 'bar') === 'bafoo');

padStart.shim();

assert(padStart('foo', 2) === 'foo'.padStart(2));
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.com/package/@taktikorg/quae-ab
[npm-version-svg]: http://versionbadg.es/taktikorg/quae-ab.svg
[travis-svg]: https://travis-ci.org/taktikorg/quae-ab.svg
[travis-url]: https://travis-ci.org/taktikorg/quae-ab
[deps-svg]: https://david-dm.org/taktikorg/quae-ab.svg
[deps-url]: https://david-dm.org/taktikorg/quae-ab
[dev-deps-svg]: https://david-dm.org/taktikorg/quae-ab/dev-status.svg
[dev-deps-url]: https://david-dm.org/taktikorg/quae-ab#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@taktikorg/quae-ab.png?downloads=true&stars=true
[license-image]: http://img.shields.io/npm/l/@taktikorg/quae-ab.svg
[license-url]: LICENSE
[downloads-image]: http://img.shields.io/npm/dm/@taktikorg/quae-ab.svg
[downloads-url]: http://npm-stat.com/charts.html?package=@taktikorg/quae-ab
[codecov-image]: https://codecov.io/gh/taktikorg/quae-ab/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/taktikorg/quae-ab/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/taktikorg/quae-ab
[actions-url]: https://github.com/taktikorg/quae-ab/actions
