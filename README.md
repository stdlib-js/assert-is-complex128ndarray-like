<!--

@license Apache-2.0

Copyright (c) 2023 The Stdlib Authors.

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


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# isComplex128ndarrayLike

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Test if a value is an [ndarray][@stdlib/ndarray/ctor]-like object containing double-precision complex floating-point numbers.



<section class="usage">

## Usage

```javascript
import isComplex128ndarrayLike from 'https://cdn.jsdelivr.net/gh/stdlib-js/assert-is-complex128ndarray-like@deno/mod.js';
```

#### isComplex128ndarrayLike( value )

Tests if a value is an [ndarray][@stdlib/ndarray/ctor]-like object whose underlying data type is `complex128`.

```javascript
import Complex128Array from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-complex128@deno/mod.js';
import ndarray from 'https://cdn.jsdelivr.net/gh/stdlib-js/ndarray-ctor@deno/mod.js';

var arr = ndarray( 'complex128', new Complex128Array( [ 0, 0, 0, 0, 0, 0, 0, 0 ] ), [ 2, 2 ], [ 2, 1 ], 0, 'row-major' );

var bool = isComplex128ndarrayLike( arr );
// returns true
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
import ndarray from 'https://cdn.jsdelivr.net/gh/stdlib-js/ndarray-ctor@deno/mod.js';
import Complex128Array from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-complex128@deno/mod.js';
import isComplex128ndarrayLike from 'https://cdn.jsdelivr.net/gh/stdlib-js/assert-is-complex128ndarray-like@deno/mod.js';

var buffer = new Complex128Array( [ 0, 0, 0, 0, 0, 0, 0, 0 ] );
var arr = ndarray( 'complex128', buffer, [ 2, 2 ], [ 2, 1 ], 0, 'row-major' );

var out = isComplex128ndarrayLike( arr );
// returns true

out = isComplex128ndarrayLike( [ 1, 2, 3, 4 ] );
// returns false

out = isComplex128ndarrayLike( {} );
// returns false

out = isComplex128ndarrayLike( null );
// returns false
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

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

[npm-image]: http://img.shields.io/npm/v/@stdlib/assert-is-complex128ndarray-like.svg
[npm-url]: https://npmjs.org/package/@stdlib/assert-is-complex128ndarray-like

[test-image]: https://github.com/stdlib-js/assert-is-complex128ndarray-like/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/assert-is-complex128ndarray-like/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/assert-is-complex128ndarray-like/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/assert-is-complex128ndarray-like?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/assert-is-complex128ndarray-like.svg
[dependencies-url]: https://david-dm.org/stdlib-js/assert-is-complex128ndarray-like/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/assert-is-complex128ndarray-like/tree/deno
[umd-url]: https://github.com/stdlib-js/assert-is-complex128ndarray-like/tree/umd
[esm-url]: https://github.com/stdlib-js/assert-is-complex128ndarray-like/tree/esm
[branches-url]: https://github.com/stdlib-js/assert-is-complex128ndarray-like/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/assert-is-complex128ndarray-like/main/LICENSE

[@stdlib/ndarray/ctor]: https://github.com/stdlib-js/ndarray-ctor/tree/deno

</section>

<!-- /.links -->
