# @turf/polygon-smooth

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

## polygonSmooth

Smooths a [Polygon][1] or [MultiPolygon][2]. Based on [Chaikin's algorithm][3].
Warning: may create degenerate polygons.

### Parameters

*   `inputPolys` **([FeatureCollection][4]<([Polygon][1] | [MultiPolygon][2])> | [Feature][5]<([Polygon][1] | [MultiPolygon][2])> | [Polygon][1] | [MultiPolygon][2])** (Multi)Polygon(s) to smooth
*   `options` **[Object][6]** Optional parameters (optional, default `{}`)

    *   `options.iterations` **[string][7]** The number of times to smooth the polygon. A higher value means a smoother polygon. (optional, default `1`)

### Examples

```javascript
var polygon = turf.polygon([[[11, 0], [22, 4], [31, 0], [31, 11], [21, 15], [11, 11], [11, 0]]]);

var smoothed = turf.polygonSmooth(polygon, {iterations: 3})

//addToMap
var addToMap = [smoothed, polygon];
```

Returns **[FeatureCollection][4]<([Polygon][1] | [MultiPolygon][2])>** FeatureCollection containing the smoothed polygon/multipoylgons

[1]: https://tools.ietf.org/html/rfc7946#section-3.1.6

[2]: https://tools.ietf.org/html/rfc7946#section-3.1.7

[3]: https://www.cs.unc.edu/~dm/UNC/COMP258/LECTURES/Chaikins-Algorithm.pdf

[4]: https://tools.ietf.org/html/rfc7946#section-3.3

[5]: https://tools.ietf.org/html/rfc7946#section-3.2

[6]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object

[7]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String

<!-- This file is automatically generated. Please don't edit it directly. If you find an error, edit the source file of the module in question (likely index.js or index.ts), and re-run "yarn docs" from the root of the turf project. -->

---

This module is part of the [Turfjs project](https://turfjs.org/), an open source module collection dedicated to geographic algorithms. It is maintained in the [Turfjs/turf](https://github.com/Turfjs/turf) repository, where you can create PRs and issues.

### Installation

Install this single module individually:

```sh
$ npm install @turf/polygon-smooth
```

Or install the all-encompassing @turf/turf module that includes all modules as functions:

```sh
$ npm install @turf/turf
```
