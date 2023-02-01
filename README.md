<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->

# cceil

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Round a double-precision complex floating-point number toward positive infinity.



<section class="usage">

## Usage

To use in Observable,

```javascript
cceil = require( 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-cceil@umd/browser.js' )
```

To vendor stdlib functionality and avoid installing dependency trees for Node.js, you can use the UMD server build:

```javascript
var cceil = require( 'path/to/vendor/umd/math-base-special-cceil/index.js' )
```

To include the bundle in a webpage,

```html
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-cceil@umd/browser.js"></script>
```

If no recognized module system is present, access bundle contents via the global scope:

```html
<script type="text/javascript">
(function () {
    window.cceil;
})();
</script>
```

#### cceil( z )

Rounds a double-precision complex floating-point number toward positive infinity.

```javascript
var Complex128 = require( '@stdlib/complex-float64' );
var real = require( '@stdlib/complex-real' );
var imag = require( '@stdlib/complex-imag' );

var v = cceil( new Complex128( -1.5, 2.5 ) );
// returns <Complex128>

var re = real( v );
// returns -1.0

var im = imag( v );
// returns 3.0
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/random-base-uniform@umd/browser.js"></script>
<script type="text/javascript">
(function () {.factory;
var Complex128 = require( '@stdlib/complex-float64' );
var cceil = require( '@stdlib/math-base-special-cceil' );

var rand = uniform( -50.0, 50.0 );

var z;
var i;
for ( i = 0; i < 100; i++ ) {
    z = new Complex128( rand(), rand() );
    console.log( 'cceil(%s) = %s', z, cceil( z ) );
}

})();
</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- C interface documentation. -->



<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/math/base/special/cceiln`][@stdlib/math/base/special/cceiln]</span><span class="delimiter">: </span><span class="description">round a complex number to the nearest multiple of 10^n toward positive infinity.</span>
-   <span class="package-name">[`@stdlib/math/base/special/cfloor`][@stdlib/math/base/special/cfloor]</span><span class="delimiter">: </span><span class="description">round a complex number toward negative infinity.</span>
-   <span class="package-name">[`@stdlib/math/base/special/cround`][@stdlib/math/base/special/cround]</span><span class="delimiter">: </span><span class="description">round a complex number to the nearest integer.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2023. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-base-special-cceil.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-base-special-cceil

[test-image]: https://github.com/stdlib-js/math-base-special-cceil/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/math-base-special-cceil/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-base-special-cceil/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-base-special-cceil?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-base-special-cceil.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-base-special-cceil/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/math-base-special-cceil/tree/deno
[umd-url]: https://github.com/stdlib-js/math-base-special-cceil/tree/umd
[esm-url]: https://github.com/stdlib-js/math-base-special-cceil/tree/esm
[branches-url]: https://github.com/stdlib-js/math-base-special-cceil/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-base-special-cceil/main/LICENSE

<!-- <related-links> -->

[@stdlib/math/base/special/cceiln]: https://github.com/stdlib-js/math-base-special-cceiln/tree/umd

[@stdlib/math/base/special/cfloor]: https://github.com/stdlib-js/math-base-special-cfloor/tree/umd

[@stdlib/math/base/special/cround]: https://github.com/stdlib-js/math-base-special-cround/tree/umd

<!-- </related-links> -->

</section>

<!-- /.links -->
