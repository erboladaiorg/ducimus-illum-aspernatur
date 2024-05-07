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


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# Arrays

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Arrays.

<section class="installation">

## Installation

```bash
npm install @erboladaiorg/ducimus-illum-aspernatur
```

Alternatively,

-   To load the package in a website via a `script` tag without installation and bundlers, use the [ES Module][es-module] available on the [`esm`][esm-url] branch (see [README][esm-readme]).
-   If you are using Deno, visit the [`deno`][deno-url] branch (see [README][deno-readme] for usage intructions).
-   For use in Observable, or in browser/node environments, use the [Universal Module Definition (UMD)][umd] build available on the [`umd`][umd-url] branch (see [README][umd-readme]).

The [branches.md][branches-url] file summarizes the available branches and displays a diagram illustrating their relationships.

To view installation and usage instructions specific to each branch build, be sure to explicitly navigate to the respective README files on each branch, as linked to above.

</section>

<section class="usage">

## Usage

```javascript
var ns = require( '@erboladaiorg/ducimus-illum-aspernatur' );
```

#### ns

Arrays.

```javascript
var o = ns;
// returns {...}
```

The namespace exports the following array constructors:

<!-- <toc pattern="+(int*|float*|uint*|*buffer)"> -->

<div class="namespace-toc">

-   <span class="signature">[`ArrayBuffer( size )`][@erboladaiorg/ducimus-illum-aspernatur/buffer]</span><span class="delimiter">: </span><span class="description">constructor which returns an object used to represent a generic, fixed-length raw binary data buffer.</span>
-   <span class="signature">[`Float32Array()`][@erboladaiorg/ducimus-illum-aspernatur/float32]</span><span class="delimiter">: </span><span class="description">typed array constructor which returns a typed array representing an array of single-precision floating-point numbers in the platform byte order.</span>
-   <span class="signature">[`Float64Array()`][@erboladaiorg/ducimus-illum-aspernatur/float64]</span><span class="delimiter">: </span><span class="description">typed array constructor which returns a typed array representing an array of double-precision floating-point numbers in the platform byte order.</span>
-   <span class="signature">[`Int16Array()`][@erboladaiorg/ducimus-illum-aspernatur/int16]</span><span class="delimiter">: </span><span class="description">typed array constructor which returns a typed array representing an array of twos-complement 16-bit signed integers in the platform byte order.</span>
-   <span class="signature">[`Int32Array()`][@erboladaiorg/ducimus-illum-aspernatur/int32]</span><span class="delimiter">: </span><span class="description">typed array constructor which returns a typed array representing an array of twos-complement 32-bit signed integers in the platform byte order.</span>
-   <span class="signature">[`Int8Array()`][@erboladaiorg/ducimus-illum-aspernatur/int8]</span><span class="delimiter">: </span><span class="description">typed array constructor which returns a typed array representing an array of twos-complement 8-bit signed integers in the platform byte order.</span>
-   <span class="signature">[`SharedArrayBuffer( size )`][@erboladaiorg/ducimus-illum-aspernatur/shared-buffer]</span><span class="delimiter">: </span><span class="description">constructor returning an object used to represent a generic, fixed-length raw binary data buffer which can be used to create views of shared memory.</span>
-   <span class="signature">[`Uint16Array()`][@erboladaiorg/ducimus-illum-aspernatur/uint16]</span><span class="delimiter">: </span><span class="description">typed array constructor which returns a typed array representing an array of 16-bit unsigned integers in the platform byte order.</span>
-   <span class="signature">[`Uint32Array()`][@erboladaiorg/ducimus-illum-aspernatur/uint32]</span><span class="delimiter">: </span><span class="description">typed array constructor which returns a typed array representing an array of 32-bit unsigned integers in the platform byte order.</span>
-   <span class="signature">[`Uint8Array()`][@erboladaiorg/ducimus-illum-aspernatur/uint8]</span><span class="delimiter">: </span><span class="description">typed array constructor which returns a typed array representing an array of 8-bit unsigned integers in the platform byte order.</span>
-   <span class="signature">[`Uint8ClampedArray()`][@erboladaiorg/ducimus-illum-aspernatur/uint8c]</span><span class="delimiter">: </span><span class="description">typed array constructor which returns a typed array representing an array of 8-bit unsigned integers in the platform byte order clamped to 0-255.</span>

</div>

<!-- </toc> -->

```javascript
var arr = new ns.Int32Array( 5 );
// returns <Int32Array>[ 0, 0, 0, 0, 0 ]
```

Alternatively, use the `typedarray` function to create a typed array of a given data type:

<!-- <toc pattern="typed"> -->

<div class="namespace-toc">

-   <span class="signature">[`typedarray()`][@erboladaiorg/ducimus-illum-aspernatur/typed]</span><span class="delimiter">: </span><span class="description">create a typed array.</span>

</div>

<!-- </toc> -->

```javascript
var arr1 = ns.typedarray( 5 );
// returns <Float64Array>[ 0.0, 0.0, 0.0, 0.0, 0.0 ]

var arr2 = ns.typedarray( 5, 'uint8' );
// returns <Uint8Array>[ 0, 0, 0, 0, 0 ]
```

The namespace contains functions to create arrays pre-filled with spaced values:

<!-- <toc pattern="*space"> -->

<div class="namespace-toc">

-   <span class="signature">[`datespace( start, stop[, length][, opts] )`][@erboladaiorg/ducimus-illum-aspernatur/datespace]</span><span class="delimiter">: </span><span class="description">generate an array of linearly spaced dates.</span>
-   <span class="signature">[`incrspace( start, stop[, increment] )`][@erboladaiorg/ducimus-illum-aspernatur/incrspace]</span><span class="delimiter">: </span><span class="description">generate a linearly spaced numeric array using a provided increment.</span>
-   <span class="signature">[`linspace( start, stop, length[, options] )`][@erboladaiorg/ducimus-illum-aspernatur/linspace]</span><span class="delimiter">: </span><span class="description">generate a linearly spaced array over a specified interval.</span>
-   <span class="signature">[`logspace( a, b[, length] )`][@erboladaiorg/ducimus-illum-aspernatur/logspace]</span><span class="delimiter">: </span><span class="description">generate a logarithmically spaced numeric array.</span>

</div>

<!-- </toc> -->

You can use the following functions to retrieve a list of available data types:

<!-- <toc pattern="*dtypes"> -->

<div class="namespace-toc">

-   <span class="signature">[`dtypes( [kind] )`][@erboladaiorg/ducimus-illum-aspernatur/dtypes]</span><span class="delimiter">: </span><span class="description">list of array data types.</span>
-   <span class="signature">[`complexarrayDataTypes()`][@erboladaiorg/ducimus-illum-aspernatur/typed-complex-dtypes]</span><span class="delimiter">: </span><span class="description">list of complex typed array data types.</span>
-   <span class="signature">[`typedarrayDataTypes()`][@erboladaiorg/ducimus-illum-aspernatur/typed-dtypes]</span><span class="delimiter">: </span><span class="description">list of typed array data types.</span>
-   <span class="signature">[`floatarrayDataTypes()`][@erboladaiorg/ducimus-illum-aspernatur/typed-float-dtypes]</span><span class="delimiter">: </span><span class="description">list of typed array floating-point data types.</span>
-   <span class="signature">[`intarrayDataTypes()`][@erboladaiorg/ducimus-illum-aspernatur/typed-integer-dtypes]</span><span class="delimiter">: </span><span class="description">list of typed array integer data types.</span>
-   <span class="signature">[`realarrayDataTypes()`][@erboladaiorg/ducimus-illum-aspernatur/typed-real-dtypes]</span><span class="delimiter">: </span><span class="description">list of typed array real-valued data types.</span>
-   <span class="signature">[`realarrayFloatDataTypes()`][@erboladaiorg/ducimus-illum-aspernatur/typed-real-float-dtypes]</span><span class="delimiter">: </span><span class="description">list of typed array real-valued floating-point data types.</span>
-   <span class="signature">[`intarraySignedDataTypes()`][@erboladaiorg/ducimus-illum-aspernatur/typed-signed-integer-dtypes]</span><span class="delimiter">: </span><span class="description">list of typed array signed integer data types.</span>
-   <span class="signature">[`intarrayUnsignedDataTypes()`][@erboladaiorg/ducimus-illum-aspernatur/typed-unsigned-integer-dtypes]</span><span class="delimiter">: </span><span class="description">list of typed array unsigned integer data types.</span>

</div>

<!-- </toc> -->

Furthermore, the namespace contains utility functions to retrieve a given constructor:

<!-- <toc keywords="+constructors,+constructor"> -->

<div class="namespace-toc">

-   <span class="signature">[`ctors( dtype )`][@erboladaiorg/ducimus-illum-aspernatur/ctors]</span><span class="delimiter">: </span><span class="description">array constructors.</span>
-   <span class="signature">[`ArrayIndex( x[, options] )`][@erboladaiorg/ducimus-illum-aspernatur/index]</span><span class="delimiter">: </span><span class="description">array index constructor.</span>
-   <span class="signature">[`complexarrayCtors( dtype )`][@erboladaiorg/ducimus-illum-aspernatur/typed-complex-ctors]</span><span class="delimiter">: </span><span class="description">complex typed array constructors.</span>
-   <span class="signature">[`typedarrayCtors( dtype )`][@erboladaiorg/ducimus-illum-aspernatur/typed-ctors]</span><span class="delimiter">: </span><span class="description">typed array constructors.</span>
-   <span class="signature">[`floatarrayCtors( dtype )`][@erboladaiorg/ducimus-illum-aspernatur/typed-float-ctors]</span><span class="delimiter">: </span><span class="description">floating-point typed array constructors.</span>
-   <span class="signature">[`intarrayCtors( dtype )`][@erboladaiorg/ducimus-illum-aspernatur/typed-integer-ctors]</span><span class="delimiter">: </span><span class="description">integer-valued typed array constructors.</span>
-   <span class="signature">[`realarrayCtors( dtype )`][@erboladaiorg/ducimus-illum-aspernatur/typed-real-ctors]</span><span class="delimiter">: </span><span class="description">typed array constructors.</span>
-   <span class="signature">[`realarrayFloatCtors( dtype )`][@erboladaiorg/ducimus-illum-aspernatur/typed-real-float-ctors]</span><span class="delimiter">: </span><span class="description">real-valued floating-point typed array constructors.</span>
-   <span class="signature">[`intarraySignedCtors( dtype )`][@erboladaiorg/ducimus-illum-aspernatur/typed-signed-integer-ctors]</span><span class="delimiter">: </span><span class="description">signed integer typed array constructors.</span>
-   <span class="signature">[`intarrayUnsignedCtors( dtype )`][@erboladaiorg/ducimus-illum-aspernatur/typed-unsigned-integer-ctors]</span><span class="delimiter">: </span><span class="description">unsigned integer typed array constructors.</span>

</div>

<!-- </toc> -->

```javascript
var ctor = ns.typedarrayCtors( 'float64' );
// returns <Function>

ctor = ns.typedarrayCtors( 'int' );
// returns null
```

Lastly, the namespace contains various other functions for dealing with arrays, including functions to convert arrays from one data type to another or to serialize them as JSON and vice versa.

<!-- <toc ignore="+(int*|float*|uint*|*buffer)" ignore="typed" ignore="*dtypes" keywords="-constructors,-constructor"> -->

<div class="namespace-toc">

-   <span class="signature">[`base`][@erboladaiorg/ducimus-illum-aspernatur/base]</span><span class="delimiter">: </span><span class="description">base (i.e., lower-level) array utilities.</span>
-   <span class="signature">[`cartesianPower( x, n )`][@erboladaiorg/ducimus-illum-aspernatur/cartesian-power]</span><span class="delimiter">: </span><span class="description">return the Cartesian power.</span>
-   <span class="signature">[`cartesianProduct( x1, x2 )`][@erboladaiorg/ducimus-illum-aspernatur/cartesian-product]</span><span class="delimiter">: </span><span class="description">return the Cartesian product.</span>
-   <span class="signature">[`cartesianSquare( x )`][@erboladaiorg/ducimus-illum-aspernatur/cartesian-square]</span><span class="delimiter">: </span><span class="description">return the Cartesian square.</span>
-   <span class="signature">[`Complex128Array()`][@erboladaiorg/ducimus-illum-aspernatur/complex128]</span><span class="delimiter">: </span><span class="description">128-bit complex number array.</span>
-   <span class="signature">[`Complex64Array()`][@erboladaiorg/ducimus-illum-aspernatur/complex64]</span><span class="delimiter">: </span><span class="description">64-bit complex number array.</span>
-   <span class="signature">[`convertSame( x, y )`][@erboladaiorg/ducimus-illum-aspernatur/convert-same]</span><span class="delimiter">: </span><span class="description">convert an array to the same data type as a second input array.</span>
-   <span class="signature">[`convert( arr, dtype )`][@erboladaiorg/ducimus-illum-aspernatur/convert]</span><span class="delimiter">: </span><span class="description">convert an array to an array of a different data type.</span>
-   <span class="signature">[`DataView( buffer[, byteOffset[, byteLength]] )`][@erboladaiorg/ducimus-illum-aspernatur/dataview]</span><span class="delimiter">: </span><span class="description">constructor which returns a data view representing a provided array buffer.</span>
-   <span class="signature">[`defaults()`][@erboladaiorg/ducimus-illum-aspernatur/defaults]</span><span class="delimiter">: </span><span class="description">default array settings.</span>
-   <span class="signature">[`dtype( array )`][@erboladaiorg/ducimus-illum-aspernatur/dtype]</span><span class="delimiter">: </span><span class="description">return the data type of an array.</span>
-   <span class="signature">[`emptyLike( x[, dtype] )`][@erboladaiorg/ducimus-illum-aspernatur/empty-like]</span><span class="delimiter">: </span><span class="description">create an uninitialized array having the same length and data type as a provided array.</span>
-   <span class="signature">[`empty( length[, dtype] )`][@erboladaiorg/ducimus-illum-aspernatur/empty]</span><span class="delimiter">: </span><span class="description">create an uninitialized array having a specified length.</span>
-   <span class="signature">[`filledBy()`][@erboladaiorg/ducimus-illum-aspernatur/filled-by]</span><span class="delimiter">: </span><span class="description">create a filled array according to a provided callback function.</span>
-   <span class="signature">[`filled()`][@erboladaiorg/ducimus-illum-aspernatur/filled]</span><span class="delimiter">: </span><span class="description">create a filled array.</span>
-   <span class="signature">[`iterator2array( iterator[, out][, mapFcn[, thisArg]] )`][@erboladaiorg/ducimus-illum-aspernatur/from-iterator]</span><span class="delimiter">: </span><span class="description">create (or fill) an array from an iterator.</span>
-   <span class="signature">[`scalar2array( value[, dtype] )`][@erboladaiorg/ducimus-illum-aspernatur/from-scalar]</span><span class="delimiter">: </span><span class="description">create a single-element array containing a provided scalar value.</span>
-   <span class="signature">[`fullLike( x, value[, dtype] )`][@erboladaiorg/ducimus-illum-aspernatur/full-like]</span><span class="delimiter">: </span><span class="description">create a filled array having the same length and data type as a provided array.</span>
-   <span class="signature">[`full( length, value[, dtype] )`][@erboladaiorg/ducimus-illum-aspernatur/full]</span><span class="delimiter">: </span><span class="description">create a filled array having a specified length.</span>
-   <span class="signature">[`minDataType( value )`][@erboladaiorg/ducimus-illum-aspernatur/min-dtype]</span><span class="delimiter">: </span><span class="description">determine the minimum array data type of the closest "kind" necessary for storing a provided scalar value.</span>
-   <span class="signature">[`mostlySafeCasts( [dtype] )`][@erboladaiorg/ducimus-illum-aspernatur/mostly-safe-casts]</span><span class="delimiter">: </span><span class="description">return a list of array data types to which a provided array data type can be safely cast and, for floating-point data types, can be downcast.</span>
-   <span class="signature">[`mskfilter( x, mask )`][@erboladaiorg/ducimus-illum-aspernatur/mskfilter]</span><span class="delimiter">: </span><span class="description">apply a mask to a provided input array.</span>
-   <span class="signature">[`mskreject( x, mask )`][@erboladaiorg/ducimus-illum-aspernatur/mskreject]</span><span class="delimiter">: </span><span class="description">apply a mask to a provided input array.</span>
-   <span class="signature">[`nansLike( x[, dtype] )`][@erboladaiorg/ducimus-illum-aspernatur/nans-like]</span><span class="delimiter">: </span><span class="description">create an array filled with NaNs and having the same length and data type as a provided array.</span>
-   <span class="signature">[`nans( length[, dtype] )`][@erboladaiorg/ducimus-illum-aspernatur/nans]</span><span class="delimiter">: </span><span class="description">create an array filled with NaNs and having a specified length.</span>
-   <span class="signature">[`nextDataType( [dtype] )`][@erboladaiorg/ducimus-illum-aspernatur/next-dtype]</span><span class="delimiter">: </span><span class="description">return the next larger array data type of the same kind.</span>
-   <span class="signature">[`oneToLike( x[, dtype] )`][@erboladaiorg/ducimus-illum-aspernatur/one-to-like]</span><span class="delimiter">: </span><span class="description">generate a linearly spaced numeric array whose elements increment by `1` starting from one and having the same length and data type as a provided input array.</span>
-   <span class="signature">[`oneTo( n[, dtype] )`][@erboladaiorg/ducimus-illum-aspernatur/one-to]</span><span class="delimiter">: </span><span class="description">generate a linearly spaced numeric array whose elements increment by `1` starting from one.</span>
-   <span class="signature">[`onesLike( x[, dtype] )`][@erboladaiorg/ducimus-illum-aspernatur/ones-like]</span><span class="delimiter">: </span><span class="description">create an array filled with ones and having the same length and data type as a provided array.</span>
-   <span class="signature">[`ones( length[, dtype] )`][@erboladaiorg/ducimus-illum-aspernatur/ones]</span><span class="delimiter">: </span><span class="description">create an array filled with ones and having a specified length.</span>
-   <span class="signature">[`typedarraypool()`][@erboladaiorg/ducimus-illum-aspernatur/pool]</span><span class="delimiter">: </span><span class="description">allocate typed arrays from a typed array memory pool.</span>
-   <span class="signature">[`promotionRules( [dtype1, dtype2] )`][@erboladaiorg/ducimus-illum-aspernatur/promotion-rules]</span><span class="delimiter">: </span><span class="description">return the array data type with the smallest size and closest "kind" to which array data types can be **safely** cast.</span>
-   <span class="signature">[`typedarrayReviver( key, value )`][@erboladaiorg/ducimus-illum-aspernatur/reviver]</span><span class="delimiter">: </span><span class="description">revive a JSON-serialized typed array.</span>
-   <span class="signature">[`safeCasts( [dtype] )`][@erboladaiorg/ducimus-illum-aspernatur/safe-casts]</span><span class="delimiter">: </span><span class="description">return a list of array data types to which a provided array data type can be safely cast.</span>
-   <span class="signature">[`sameKindCasts( [dtype] )`][@erboladaiorg/ducimus-illum-aspernatur/same-kind-casts]</span><span class="delimiter">: </span><span class="description">return a list of array data types to which a provided array data type can be safely cast or cast within the same "kind".</span>
-   <span class="signature">[`shape( arr )`][@erboladaiorg/ducimus-illum-aspernatur/shape]</span><span class="delimiter">: </span><span class="description">determine (nested) array dimensions.</span>
-   <span class="signature">[`slice( x[, start[, end]] )`][@erboladaiorg/ducimus-illum-aspernatur/slice]</span><span class="delimiter">: </span><span class="description">return a shallow copy of a portion of an array.</span>
-   <span class="signature">[`take( x, indices[, options] )`][@erboladaiorg/ducimus-illum-aspernatur/take]</span><span class="delimiter">: </span><span class="description">take elements from an array.</span>
-   <span class="signature">[`circarray2iterator( src[, options][, mapFcn[, thisArg]] )`][@erboladaiorg/ducimus-illum-aspernatur/to-circular-iterator]</span><span class="delimiter">: </span><span class="description">create an iterator which repeatedly iterates over the elements of an array-like object.</span>
-   <span class="signature">[`array2fancy( x[, options] )`][@erboladaiorg/ducimus-illum-aspernatur/to-fancy]</span><span class="delimiter">: </span><span class="description">convert an array to an object supporting fancy indexing.</span>
-   <span class="signature">[`array2iteratorRight( src[, mapFcn[, thisArg]] )`][@erboladaiorg/ducimus-illum-aspernatur/to-iterator-right]</span><span class="delimiter">: </span><span class="description">create an iterator from an array-like object, iterating from right to left.</span>
-   <span class="signature">[`array2iterator( src[, mapFcn[, thisArg]] )`][@erboladaiorg/ducimus-illum-aspernatur/to-iterator]</span><span class="delimiter">: </span><span class="description">create an iterator from an array-like object.</span>
-   <span class="signature">[`typedarray2json( typedarray )`][@erboladaiorg/ducimus-illum-aspernatur/to-json]</span><span class="delimiter">: </span><span class="description">return a JSON representation of a typed array.</span>
-   <span class="signature">[`sparsearray2iteratorRight( src[, mapFcn[, thisArg]] )`][@erboladaiorg/ducimus-illum-aspernatur/to-sparse-iterator-right]</span><span class="delimiter">: </span><span class="description">create an iterator from a sparse array-like object, iterating from right to left.</span>
-   <span class="signature">[`sparsearray2iterator( src[, mapFcn[, thisArg]] )`][@erboladaiorg/ducimus-illum-aspernatur/to-sparse-iterator]</span><span class="delimiter">: </span><span class="description">create an iterator from a sparse array-like object.</span>
-   <span class="signature">[`stridedarray2iterator( N, src, stride, offset[, mapFcn[, thisArg]] )`][@erboladaiorg/ducimus-illum-aspernatur/to-strided-iterator]</span><span class="delimiter">: </span><span class="description">create an iterator from a strided array-like object.</span>
-   <span class="signature">[`arrayview2iteratorRight( src[, begin[, end]][, mapFcn[, thisArg]] )`][@erboladaiorg/ducimus-illum-aspernatur/to-view-iterator-right]</span><span class="delimiter">: </span><span class="description">create an iterator from an array-like object view, iterating from right to left.</span>
-   <span class="signature">[`arrayview2iterator( src[, begin[, end]][, mapFcn[, thisArg]] )`][@erboladaiorg/ducimus-illum-aspernatur/to-view-iterator]</span><span class="delimiter">: </span><span class="description">create an iterator from an array-like object view.</span>
-   <span class="signature">[`complexarray()`][@erboladaiorg/ducimus-illum-aspernatur/typed-complex]</span><span class="delimiter">: </span><span class="description">create a complex number typed array.</span>
-   <span class="signature">[`realarray()`][@erboladaiorg/ducimus-illum-aspernatur/typed-real]</span><span class="delimiter">: </span><span class="description">create a typed array.</span>
-   <span class="signature">[`zeroToLike( x[, dtype] )`][@erboladaiorg/ducimus-illum-aspernatur/zero-to-like]</span><span class="delimiter">: </span><span class="description">generate a linearly spaced numeric array whose elements increment by `1` starting from zero and having the same length and data type as a provided input array.</span>
-   <span class="signature">[`zeroTo( n[, dtype] )`][@erboladaiorg/ducimus-illum-aspernatur/zero-to]</span><span class="delimiter">: </span><span class="description">generate a linearly spaced numeric array whose elements increment by `1` starting from zero.</span>
-   <span class="signature">[`zerosLike( x[, dtype] )`][@erboladaiorg/ducimus-illum-aspernatur/zeros-like]</span><span class="delimiter">: </span><span class="description">create a zero-filled array having the same length and data type as a provided array.</span>
-   <span class="signature">[`zeros( length[, dtype] )`][@erboladaiorg/ducimus-illum-aspernatur/zeros]</span><span class="delimiter">: </span><span class="description">create a zero-filled array having a specified length.</span>

</div>

<!-- </toc> -->

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- TODO: better examples -->

<!-- eslint no-undef: "error" -->

```javascript
var objectKeys = require( '@stdlib/utils/keys' );
var ns = require( '@erboladaiorg/ducimus-illum-aspernatur' );

console.log( objectKeys( ns ) );
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

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2024. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@erboladaiorg/ducimus-illum-aspernatur.svg
[npm-url]: https://npmjs.org/package/@erboladaiorg/ducimus-illum-aspernatur

[test-image]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/erboladaiorg/ducimus-illum-aspernatur/main.svg
[coverage-url]: https://codecov.io/github/erboladaiorg/ducimus-illum-aspernatur?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/erboladaiorg/ducimus-illum-aspernatur.svg
[dependencies-url]: https://david-dm.org/erboladaiorg/ducimus-illum-aspernatur/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/deno
[deno-readme]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/blob/deno/README.md
[umd-url]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/umd
[umd-readme]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/blob/umd/README.md
[esm-url]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/esm
[esm-readme]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/blob/esm/README.md
[branches-url]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/erboladaiorg/ducimus-illum-aspernatur/main/LICENSE

<!-- <toc-links> -->

[@erboladaiorg/ducimus-illum-aspernatur/base]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/base

[@erboladaiorg/ducimus-illum-aspernatur/cartesian-power]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/cartesian-power

[@erboladaiorg/ducimus-illum-aspernatur/cartesian-product]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/cartesian-product

[@erboladaiorg/ducimus-illum-aspernatur/cartesian-square]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/cartesian-square

[@erboladaiorg/ducimus-illum-aspernatur/complex128]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/complex128

[@erboladaiorg/ducimus-illum-aspernatur/complex64]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/complex64

[@erboladaiorg/ducimus-illum-aspernatur/convert-same]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/convert-same

[@erboladaiorg/ducimus-illum-aspernatur/convert]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/convert

[@erboladaiorg/ducimus-illum-aspernatur/dataview]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/dataview

[@erboladaiorg/ducimus-illum-aspernatur/defaults]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/defaults

[@erboladaiorg/ducimus-illum-aspernatur/dtype]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/dtype

[@erboladaiorg/ducimus-illum-aspernatur/empty-like]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/empty-like

[@erboladaiorg/ducimus-illum-aspernatur/empty]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/empty

[@erboladaiorg/ducimus-illum-aspernatur/filled-by]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/filled-by

[@erboladaiorg/ducimus-illum-aspernatur/filled]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/filled

[@erboladaiorg/ducimus-illum-aspernatur/from-iterator]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/from-iterator

[@erboladaiorg/ducimus-illum-aspernatur/from-scalar]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/from-scalar

[@erboladaiorg/ducimus-illum-aspernatur/full-like]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/full-like

[@erboladaiorg/ducimus-illum-aspernatur/full]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/full

[@erboladaiorg/ducimus-illum-aspernatur/min-dtype]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/min-dtype

[@erboladaiorg/ducimus-illum-aspernatur/mostly-safe-casts]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/mostly-safe-casts

[@erboladaiorg/ducimus-illum-aspernatur/mskfilter]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/mskfilter

[@erboladaiorg/ducimus-illum-aspernatur/mskreject]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/mskreject

[@erboladaiorg/ducimus-illum-aspernatur/nans-like]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/nans-like

[@erboladaiorg/ducimus-illum-aspernatur/nans]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/nans

[@erboladaiorg/ducimus-illum-aspernatur/next-dtype]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/next-dtype

[@erboladaiorg/ducimus-illum-aspernatur/one-to-like]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/one-to-like

[@erboladaiorg/ducimus-illum-aspernatur/one-to]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/one-to

[@erboladaiorg/ducimus-illum-aspernatur/ones-like]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/ones-like

[@erboladaiorg/ducimus-illum-aspernatur/ones]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/ones

[@erboladaiorg/ducimus-illum-aspernatur/pool]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/pool

[@erboladaiorg/ducimus-illum-aspernatur/promotion-rules]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/promotion-rules

[@erboladaiorg/ducimus-illum-aspernatur/reviver]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/reviver

[@erboladaiorg/ducimus-illum-aspernatur/safe-casts]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/safe-casts

[@erboladaiorg/ducimus-illum-aspernatur/same-kind-casts]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/same-kind-casts

[@erboladaiorg/ducimus-illum-aspernatur/shape]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/shape

[@erboladaiorg/ducimus-illum-aspernatur/slice]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/slice

[@erboladaiorg/ducimus-illum-aspernatur/take]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/take

[@erboladaiorg/ducimus-illum-aspernatur/to-circular-iterator]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/to-circular-iterator

[@erboladaiorg/ducimus-illum-aspernatur/to-fancy]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/to-fancy

[@erboladaiorg/ducimus-illum-aspernatur/to-iterator-right]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/to-iterator-right

[@erboladaiorg/ducimus-illum-aspernatur/to-iterator]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/to-iterator

[@erboladaiorg/ducimus-illum-aspernatur/to-json]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/to-json

[@erboladaiorg/ducimus-illum-aspernatur/to-sparse-iterator-right]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/to-sparse-iterator-right

[@erboladaiorg/ducimus-illum-aspernatur/to-sparse-iterator]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/to-sparse-iterator

[@erboladaiorg/ducimus-illum-aspernatur/to-strided-iterator]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/to-strided-iterator

[@erboladaiorg/ducimus-illum-aspernatur/to-view-iterator-right]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/to-view-iterator-right

[@erboladaiorg/ducimus-illum-aspernatur/to-view-iterator]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/to-view-iterator

[@erboladaiorg/ducimus-illum-aspernatur/typed-complex]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/typed-complex

[@erboladaiorg/ducimus-illum-aspernatur/typed-real]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/typed-real

[@erboladaiorg/ducimus-illum-aspernatur/zero-to-like]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/zero-to-like

[@erboladaiorg/ducimus-illum-aspernatur/zero-to]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/zero-to

[@erboladaiorg/ducimus-illum-aspernatur/zeros-like]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/zeros-like

[@erboladaiorg/ducimus-illum-aspernatur/zeros]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/zeros

[@erboladaiorg/ducimus-illum-aspernatur/ctors]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/ctors

[@erboladaiorg/ducimus-illum-aspernatur/index]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/index

[@erboladaiorg/ducimus-illum-aspernatur/typed-complex-ctors]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/typed-complex-ctors

[@erboladaiorg/ducimus-illum-aspernatur/typed-ctors]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/typed-ctors

[@erboladaiorg/ducimus-illum-aspernatur/typed-float-ctors]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/typed-float-ctors

[@erboladaiorg/ducimus-illum-aspernatur/typed-integer-ctors]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/typed-integer-ctors

[@erboladaiorg/ducimus-illum-aspernatur/typed-real-ctors]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/typed-real-ctors

[@erboladaiorg/ducimus-illum-aspernatur/typed-real-float-ctors]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/typed-real-float-ctors

[@erboladaiorg/ducimus-illum-aspernatur/typed-signed-integer-ctors]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/typed-signed-integer-ctors

[@erboladaiorg/ducimus-illum-aspernatur/typed-unsigned-integer-ctors]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/typed-unsigned-integer-ctors

[@erboladaiorg/ducimus-illum-aspernatur/dtypes]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/dtypes

[@erboladaiorg/ducimus-illum-aspernatur/typed-complex-dtypes]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/typed-complex-dtypes

[@erboladaiorg/ducimus-illum-aspernatur/typed-dtypes]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/typed-dtypes

[@erboladaiorg/ducimus-illum-aspernatur/typed-float-dtypes]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/typed-float-dtypes

[@erboladaiorg/ducimus-illum-aspernatur/typed-integer-dtypes]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/typed-integer-dtypes

[@erboladaiorg/ducimus-illum-aspernatur/typed-real-dtypes]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/typed-real-dtypes

[@erboladaiorg/ducimus-illum-aspernatur/typed-real-float-dtypes]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/typed-real-float-dtypes

[@erboladaiorg/ducimus-illum-aspernatur/typed-signed-integer-dtypes]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/typed-signed-integer-dtypes

[@erboladaiorg/ducimus-illum-aspernatur/typed-unsigned-integer-dtypes]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/typed-unsigned-integer-dtypes

[@erboladaiorg/ducimus-illum-aspernatur/datespace]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/datespace

[@erboladaiorg/ducimus-illum-aspernatur/incrspace]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/incrspace

[@erboladaiorg/ducimus-illum-aspernatur/linspace]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/linspace

[@erboladaiorg/ducimus-illum-aspernatur/logspace]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/logspace

[@erboladaiorg/ducimus-illum-aspernatur/typed]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/typed

[@erboladaiorg/ducimus-illum-aspernatur/buffer]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/buffer

[@erboladaiorg/ducimus-illum-aspernatur/float32]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/float32

[@erboladaiorg/ducimus-illum-aspernatur/float64]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/float64

[@erboladaiorg/ducimus-illum-aspernatur/int16]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/int16

[@erboladaiorg/ducimus-illum-aspernatur/int32]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/int32

[@erboladaiorg/ducimus-illum-aspernatur/int8]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/int8

[@erboladaiorg/ducimus-illum-aspernatur/shared-buffer]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/shared-buffer

[@erboladaiorg/ducimus-illum-aspernatur/uint16]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/uint16

[@erboladaiorg/ducimus-illum-aspernatur/uint32]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/uint32

[@erboladaiorg/ducimus-illum-aspernatur/uint8]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/uint8

[@erboladaiorg/ducimus-illum-aspernatur/uint8c]: https://github.com/erboladaiorg/ducimus-illum-aspernatur/tree/main/uint8c

<!-- </toc-links> -->

</section>

<!-- /.links -->
