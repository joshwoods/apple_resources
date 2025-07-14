

- Accelerate
-  cblas_drotmg(\_:\_:\_:\_:\_:) 

Function

# cblas_drotmg(\_:\_:\_:\_:\_:)

Generates a modified Givens rotation matrix.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func cblas_drotmg(
    _ D1: UnsafeMutablePointer,
    _ D2: UnsafeMutablePointer,
    _ B1: UnsafeMutablePointer,
    _ B2: Double,
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

### Double-precision float matrix functions

func cblas_dasum(__LAPACK_int, UnsafePointer&lt;Double>?, __LAPACK_int) -> Double

Computes the sum of the absolute values of elements in a vector (double-precision).

func cblas_daxpy(__LAPACK_int, Double, UnsafePointer&lt;Double>?, __LAPACK_int, UnsafeMutablePointer&lt;Double>?, __LAPACK_int)

Computes a constant times a vector plus a vector (double-precision).

func cblas_dcopy(__LAPACK_int, UnsafePointer&lt;Double>?, __LAPACK_int, UnsafeMutablePointer&lt;Double>?, __LAPACK_int)

Copies a vector to another vector (double-precision).

func cblas_dgbmv(CBLAS_ORDER, CBLAS_TRANSPOSE, __LAPACK_int, __LAPACK_int, __LAPACK_int, __LAPACK_int, Double, UnsafePointer&lt;Double>?, __LAPACK_int, UnsafePointer&lt;Double>?, __LAPACK_int, Double, UnsafeMutablePointer&lt;Double>?, __LAPACK_int)

Scales a general band matrix, then multiplies by a vector, then adds a vector (double precision).

func cblas_dgemm(CBLAS_ORDER, CBLAS_TRANSPOSE, CBLAS_TRANSPOSE, __LAPACK_int, __LAPACK_int, __LAPACK_int, Double, UnsafePointer&lt;Double>?, __LAPACK_int, UnsafePointer&lt;Double>?, __LAPACK_int, Double, UnsafeMutablePointer&lt;Double>?, __LAPACK_int)

Multiplies two matrices (double-precision).

func cblas_dgemv(CBLAS_ORDER, CBLAS_TRANSPOSE, __LAPACK_int, __LAPACK_int, Double, UnsafePointer&lt;Double>?, __LAPACK_int, UnsafePointer&lt;Double>?, __LAPACK_int, Double, UnsafeMutablePointer&lt;Double>?, __LAPACK_int)

Multiplies a matrix by a vector (double precision).

func cblas_dger(CBLAS_ORDER, __LAPACK_int, __LAPACK_int, Double, UnsafePointer&lt;Double>?, __LAPACK_int, UnsafePointer&lt;Double>?, __LAPACK_int, UnsafeMutablePointer&lt;Double>?, __LAPACK_int)

Multiplies vector X by the transpose of vector Y, then adds matrix A (double precison).

func cblas_dnrm2(__LAPACK_int, UnsafePointer&lt;Double>?, __LAPACK_int) -> Double

Computes the L2 norm (Euclidian length) of a vector (double precision).

func cblas_drot(__LAPACK_int, UnsafeMutablePointer&lt;Double>?, __LAPACK_int, UnsafeMutablePointer&lt;Double>?, __LAPACK_int, Double, Double)

Applies a Givens rotation matrix to a pair of vectors.

func cblas_drotg(UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>)

Constructs a Givens rotation matrix.

func cblas_drotm(__LAPACK_int, UnsafeMutablePointer&lt;Double>?, __LAPACK_int, UnsafeMutablePointer&lt;Double>?, __LAPACK_int, UnsafePointer&lt;Double>)

Applies a modified Givens transformation (single precision).

func cblas_dsbmv(CBLAS_ORDER, CBLAS_UPLO, __LAPACK_int, __LAPACK_int, Double, UnsafePointer&lt;Double>?, __LAPACK_int, UnsafePointer&lt;Double>?, __LAPACK_int, Double, UnsafeMutablePointer&lt;Double>?, __LAPACK_int)

Scales a symmetric band matrix, then multiplies by a vector, then adds a vector (double precision).

func cblas_dscal(__LAPACK_int, Double, UnsafeMutablePointer&lt;Double>?, __LAPACK_int)

Multiplies each element of a vector by a constant (double-precision).

func cblas_dspmv(CBLAS_ORDER, CBLAS_UPLO, __LAPACK_int, Double, UnsafePointer&lt;Double>?, UnsafePointer&lt;Double>?, __LAPACK_int, Double, UnsafeMutablePointer&lt;Double>?, __LAPACK_int)

Scales a packed symmetric matrix, then multiplies by a vector, then scales and adds another vector (double precision).

func cblas_dspr(CBLAS_ORDER, CBLAS_UPLO, __LAPACK_int, Double, UnsafePointer&lt;Double>?, __LAPACK_int, UnsafeMutablePointer&lt;Double>?)

Rank one update: adds a packed symmetric matrix to the product of a scaling factor, a vector, and its transpose (double precision).

