# @patrtorg/ratione-nobis <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

Get the byte length of an ArrayBuffer, even in engines without a `.byteLength` method.

## Example

```js
const assert = require('assert');
const byteLength = require('@patrtorg/ratione-nobis');

assert.equal(byteLength([]), NaN, 'an array is not an ArrayBuffer, yields NaN');

assert.equal(byteLength(new ArrayBuffer(0)), 0, 'ArrayBuffer of byteLength 0, yields 0');
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@patrtorg/ratione-nobis
[npm-version-svg]: https://versionbadg.es/inspect-js/@patrtorg/ratione-nobis.svg
[deps-svg]: https://david-dm.org/inspect-js/@patrtorg/ratione-nobis.svg
[deps-url]: https://david-dm.org/inspect-js/@patrtorg/ratione-nobis
[dev-deps-svg]: https://david-dm.org/inspect-js/@patrtorg/ratione-nobis/dev-status.svg
[dev-deps-url]: https://david-dm.org/inspect-js/@patrtorg/ratione-nobis#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@patrtorg/ratione-nobis.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@patrtorg/ratione-nobis.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@patrtorg/ratione-nobis.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@patrtorg/ratione-nobis
[codecov-image]: https://codecov.io/gh/inspect-js/@patrtorg/ratione-nobis/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@patrtorg/ratione-nobis/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@patrtorg/ratione-nobis
[actions-url]: https://github.com/patrtorg/ratione-nobis/actions
