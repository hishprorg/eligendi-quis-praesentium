# @hishprorg/eligendi-quis-praesentium <sup>[![Version Badge][2]][1]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![dependency status][5]][6]
[![dev dependency status][7]][8]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][11]][1]

Gets the description of a Symbol. Handles `Symbol()` vs `Symbol('')` properly when possible.

## Example

```js
var getSymbolDescription = require('@hishprorg/eligendi-quis-praesentium');
var assert = require('assert');

assert(getSymbolDescription(Symbol()) === undefined);
assert(getSymbolDescription(Symbol('')) === ''); // or `undefined`, if in an engine that lacks name inference from concise method
assert(getSymbolDescription(Symbol('foo')) === 'foo');
assert(getSymbolDescription(Symbol.iterator) === 'Symbol.iterator');
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[1]: https://npmjs.org/package/@hishprorg/eligendi-quis-praesentium
[2]: https://versionbadg.es/inspect-js/@hishprorg/eligendi-quis-praesentium.svg
[5]: https://david-dm.org/inspect-js/@hishprorg/eligendi-quis-praesentium.svg
[6]: https://david-dm.org/inspect-js/@hishprorg/eligendi-quis-praesentium
[7]: https://david-dm.org/inspect-js/@hishprorg/eligendi-quis-praesentium/dev-status.svg
[8]: https://david-dm.org/inspect-js/@hishprorg/eligendi-quis-praesentium#info=devDependencies
[11]: https://nodei.co/npm/@hishprorg/eligendi-quis-praesentium.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@hishprorg/eligendi-quis-praesentium.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@hishprorg/eligendi-quis-praesentium.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@hishprorg/eligendi-quis-praesentium
[codecov-image]: https://codecov.io/gh/inspect-js/@hishprorg/eligendi-quis-praesentium/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@hishprorg/eligendi-quis-praesentium/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@hishprorg/eligendi-quis-praesentium
[actions-url]: https://github.com/hishprorg/eligendi-quis-praesentium/actions
