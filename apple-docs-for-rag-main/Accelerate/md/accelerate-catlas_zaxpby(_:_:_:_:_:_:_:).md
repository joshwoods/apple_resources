

- Accelerate
-  catlas_zaxpby(\_:\_:\_:\_:\_:\_:\_:) 

Function

# catlas_zaxpby(\_:\_:\_:\_:\_:\_:\_:)

Computes the sum of two vectors, scaling each one separately (double-precision complex).

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func catlas_zaxpby(
    _ N: __LAPACK_int,
    _ ALPHA: OpaquePointer,
    _ X: OpaquePointer?,
    _ INCX: __LAPACK_int,
    _ BETA: OpaquePointer,
    _ Y: OpaquePointer?,
    _ INCY: __LAPACK_int
)
```

## Parameters 

`N`  

Number of elements in the vector.

`ALPHA`  

Scaling factor for `X`.

`X`  

Input vector `X`.

`INCX`  

Stride within `X`. For example, if `incX` is 7, every 7th element is used.

`BETA`  

Scaling factor for Y.

`Y`  

Input vector `Y`.

`INCY`  

Stride within `Y`. For example, if `incY` is 7, every 7th element is used.

## Discussion

On return, the contents of vector `Y` are replaced with the result.

Important

Apple provides the BLAS and LAPACK libraries under the Accelerate framework to be in line with LAPACK 3.9.1. Starting with iOS 18, iPadOS 18, macOS 15, tvOS 18, watchOS 18, and visionOS 2, the libraries are in line with LAPACK 3.11.0. These new interfaces provide additional functionality, as well as a new ILP64 interface. To use the new interfaces, define `ACCELERATE_NEW_LAPACK` before including the Accelerate or vecLib headers. For ILP64 interfaces, also define `ACCELERATE_LAPACK_ILP64`. For Swift projects, specify `ACCELERATE_NEW_LAPACK=1` and `ACCELERATE_LAPACK_ILP64=1` as preprocessor macros in Xcode build settings.

## See Also

### CATLAS and CBLAS vector functions

func catlas_caxpby(__LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int)

Computes the product of two vectors, scaling each one separately (single-precision complex).

func catlas_cset(__LAPACK_int, OpaquePointer, OpaquePointer, __LAPACK_int)

Modifies a vector (single-precision complex) in place, setting each element to a given value.

func catlas_daxpby(__LAPACK_int, Double, UnsafePointer&lt;Double>?, __LAPACK_int, Double, UnsafeMutablePointer&lt;Double>?, __LAPACK_int)

Computes the sum of two vectors, scaling each one separately (double-precision).

func catlas_dset(__LAPACK_int, Double, UnsafeMutablePointer&lt;Double>, __LAPACK_int)

Modifies a vector (double-precision) in place, setting each element to a given value.

func catlas_saxpby(__LAPACK_int, Float, UnsafePointer&lt;Float>?, __LAPACK_int, Float, UnsafeMutablePointer&lt;Float>?, __LAPACK_int)

Computes the sum of two vectors, scaling each one separately (single-precision).

func catlas_sset(__LAPACK_int, Float, UnsafeMutablePointer&lt;Float>, __LAPACK_int)

Modifies a vector (single-precision) in place, setting each element to a given value.

func catlas_zset(__LAPACK_int, OpaquePointer, OpaquePointer, __LAPACK_int)

Modifies a vector (double-precision complex) in place, setting each element to a given value.

func cblas_sdot(__LAPACK_int, UnsafePointer&lt;Float>?, __LAPACK_int, UnsafePointer&lt;Float>?, __LAPACK_int) -> Float

Computes the dot product of two vectors (single-precision).

func cblas_sdsdot(__LAPACK_int, Float, UnsafePointer&lt;Float>?, __LAPACK_int, UnsafePointer&lt;Float>?, __LAPACK_int) -> Float

Computes the dot product of two single-precision vectors plus an initial single-precision value.

func cblas_cdotc_sub(__LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer)

Calculates the dot product of the complex conjugate of a single-precision complex vector with a second single-precision complex vector.

func cblas_cdotu_sub(__LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer)

Computes the dot product of two single-precision complex vectors.

func cblas_ddot(__LAPACK_int, UnsafePointer&lt;Double>?, __LAPACK_int, UnsafePointer&lt;Double>?, __LAPACK_int) -> Double

Computes the dot product of two vectors (double-precision).

func cblas_dsdot(__LAPACK_int, UnsafePointer&lt;Float>?, __LAPACK_int, UnsafePointer&lt;Float>?, __LAPACK_int) -> Double

Computes the double-precision dot product of a pair of single-precision vectors.

func cblas_zdotc_sub(__LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer)

Calculates the dot product of the complex conjugate of a double-precision complex vector with a second double-precision complex vector.

func cblas_zdotu_sub(__LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer)

Computes the dot product of two double-precision complex vectors.

