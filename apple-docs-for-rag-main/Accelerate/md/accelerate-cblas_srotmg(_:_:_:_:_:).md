

- Accelerate
-  cblas_srotmg(\_:\_:\_:\_:\_:) 

Function

# cblas_srotmg(\_:\_:\_:\_:\_:)

Generates a modified Givens rotation matrix.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func cblas_srotmg(
    _ D1: UnsafeMutablePointer,
    _ D2: UnsafeMutablePointer,
    _ B1: UnsafeMutablePointer,
    _ B2: Float,
    _ P: UnsafeMutablePointer
)
```

## Parameters 

`D1`  

Scaling factor `D1`.

`D2`  

Scaling factor `D2`.

`B1`  

Scaling factor `B1`.

`B2`  

Scaling factor `B2`.

`P`  

A 5-element vector:

`P[0]`  
Flag value that defines the form of matrix `H`.

`-2.0`: matrix `H` contains the identity matrix.

`-1.0`: matrix `H` is identical to matrix `SH` (defined by the remaining values in the vector).

`0.0`: `H[1,2]` and `H[2,1]` are obtained from matrix `SH`. The remaining values are both `1.0`.

`1.0`: `H[1,1]` and `H[2,2]` are obtained from matrix `SH`. `H[1,2]` is 1.0. `H[2,1]` is -1.0.

`P[1]`  
Contains `SH[1,1]`.

`P[2]`  
Contains `SH[2,1]`.

`P[3]`  
Contains `SH[1,2]`.

`P[4]`  
Contains `SH[2,2]`.

## Discussion

The resulting matrix zeroes the second component of the vector `(sqrt(D1)*B1, sqrt(SD2)*B2)`.

Important

Apple provides the BLAS and LAPACK libraries under the Accelerate framework to be in line with LAPACK 3.9.1. Starting with iOS 18, iPadOS 18, macOS 15, tvOS 18, watchOS 18, and visionOS 2, the libraries are in line with LAPACK 3.11.0. These new interfaces provide additional functionality, as well as a new ILP64 interface. To use the new interfaces, define `ACCELERATE_NEW_LAPACK` before including the Accelerate or vecLib headers. For ILP64 interfaces, also define `ACCELERATE_LAPACK_ILP64`. For Swift projects, specify `ACCELERATE_NEW_LAPACK=1` and `ACCELERATE_LAPACK_ILP64=1` as preprocessor macros in Xcode build settings.

## See Also

### Single-precision float matrix functions

func cblas_sasum(__LAPACK_int, UnsafePointer&lt;Float>?, __LAPACK_int) -> Float

Computes the sum of the absolute values of elements in a vector (single-precision).

func cblas_saxpy(__LAPACK_int, Float, UnsafePointer&lt;Float>?, __LAPACK_int, UnsafeMutablePointer&lt;Float>?, __LAPACK_int)

Computes a constant times a vector plus a vector (single-precision).

func cblas_scopy(__LAPACK_int, UnsafePointer&lt;Float>?, __LAPACK_int, UnsafeMutablePointer&lt;Float>?, __LAPACK_int)

Copies a vector to another vector (single-precision).

func cblas_sgbmv(CBLAS_ORDER, CBLAS_TRANSPOSE, __LAPACK_int, __LAPACK_int, __LAPACK_int, __LAPACK_int, Float, UnsafePointer&lt;Float>?, __LAPACK_int, UnsafePointer&lt;Float>?, __LAPACK_int, Float, UnsafeMutablePointer&lt;Float>?, __LAPACK_int)

Scales a general band matrix, then multiplies by a vector, then adds a vector (single precision).

func cblas_sgemm(CBLAS_ORDER, CBLAS_TRANSPOSE, CBLAS_TRANSPOSE, __LAPACK_int, __LAPACK_int, __LAPACK_int, Float, UnsafePointer&lt;Float>?, __LAPACK_int, UnsafePointer&lt;Float>?, __LAPACK_int, Float, UnsafeMutablePointer&lt;Float>?, __LAPACK_int)

Multiplies two matrices (single-precision).

func cblas_sgemv(CBLAS_ORDER, CBLAS_TRANSPOSE, __LAPACK_int, __LAPACK_int, Float, UnsafePointer&lt;Float>?, __LAPACK_int, UnsafePointer&lt;Float>?, __LAPACK_int, Float, UnsafeMutablePointer&lt;Float>?, __LAPACK_int)

Multiplies a single-precision matrix by a vector.

func cblas_sger(CBLAS_ORDER, __LAPACK_int, __LAPACK_int, Float, UnsafePointer&lt;Float>?, __LAPACK_int, UnsafePointer&lt;Float>?, __LAPACK_int, UnsafeMutablePointer&lt;Float>?, __LAPACK_int)

Multiplies vector X by the transpose of vector Y, then adds matrix A (single precison).

func cblas_snrm2(__LAPACK_int, UnsafePointer&lt;Float>?, __LAPACK_int) -> Float

Computes the L2 norm (Euclidian length) of a vector (single precision).

func cblas_srot(__LAPACK_int, UnsafeMutablePointer&lt;Float>?, __LAPACK_int, UnsafeMutablePointer&lt;Float>?, __LAPACK_int, Float, Float)

Applies a Givens rotation matrix to a pair of vectors.

func cblas_srotg(UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>)

Constructs a Givens rotation matrix.

func cblas_srotm(__LAPACK_int, UnsafeMutablePointer&lt;Float>?, __LAPACK_int, UnsafeMutablePointer&lt;Float>?, __LAPACK_int, UnsafePointer&lt;Float>)

Applies a modified Givens transformation (single precision).

func cblas_ssbmv(CBLAS_ORDER, CBLAS_UPLO, __LAPACK_int, __LAPACK_int, Float, UnsafePointer&lt;Float>?, __LAPACK_int, UnsafePointer&lt;Float>?, __LAPACK_int, Float, UnsafeMutablePointer&lt;Float>?, __LAPACK_int)

Scales a symmetric band matrix, then multiplies by a vector, then adds a vector (single-precision).

func cblas_sscal(__LAPACK_int, Float, UnsafeMutablePointer&lt;Float>?, __LAPACK_int)

Multiplies each element of a vector by a constant (single-precision).

func cblas_sspmv(CBLAS_ORDER, CBLAS_UPLO, __LAPACK_int, Float, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, __LAPACK_int, Float, UnsafeMutablePointer&lt;Float>?, __LAPACK_int)

Scales a packed symmetric matrix, then multiplies by a vector, then scales and adds another vector (single precision).

func cblas_sspr(CBLAS_ORDER, CBLAS_UPLO, __LAPACK_int, Float, UnsafePointer&lt;Float>?, __LAPACK_int, UnsafeMutablePointer&lt;Float>?)

Rank one update: adds a packed symmetric matrix to the product of a scaling factor, a vector, and its transpose (single precision).

