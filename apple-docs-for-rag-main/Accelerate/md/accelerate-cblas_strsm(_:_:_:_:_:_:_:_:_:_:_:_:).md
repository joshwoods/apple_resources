

- Accelerate
-  cblas_strsm(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# cblas_strsm(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Solves a triangular system of equations with multiple values for the right side.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func cblas_strsm(
    _ ORDER: CBLAS_ORDER,
    _ SIDE: CBLAS_SIDE,
    _ UPLO: CBLAS_UPLO,
    _ TRANSA: CBLAS_TRANSPOSE,
    _ DIAG: CBLAS_DIAG,
    _ M: __LAPACK_int,
    _ N: __LAPACK_int,
    _ ALPHA: Float,
    _ A: UnsafePointer?,
    _ LDA: __LAPACK_int,
    _ B: UnsafeMutablePointer?,
    _ LDB: __LAPACK_int
)
```

## Parameters 

`ORDER`  

Specifies row-major (C) or column-major (Fortran) data ordering.

`SIDE`  

Determines the order in which the matrix and vector should be multiplied.

`UPLO`  

Specifies whether to use the upper or lower triangle from the matrix. Valid values are `'U'` or `'L'`.

`TRANSA`  

Specifies whether to use matrix A (`'N'` or `'n'`) or the transpose of A (`'T'`, `'t'`, `'C'`, or `'c'`).

`DIAG`  

Specifies whether the matrix is unit triangular. Possible values are `'U'` (unit triangular) or `'N'` (not unit triangular).

`M`  

The number of rows in matrix `B`.

`N`  

The number of columns in matrix `B`.

`ALPHA`  

Scaling factor for matrix `A`.

`A`  

Triangular matrix `A`.

`LDA`  

The leading dimension of matrix `A`.

`B`  

On entry, matrix `B`. Overwritten on return by matrix `X`.

`LDB`  

The leading dimension of matrix `B`.

## Discussion

If `Side` is `'L'`, solves `A*X=alpha*B` or `A'*X=alpha*B`, depending on `TransA`.

If `Side` is `'R'`, solves `X*A=alpha*B` or `X*A'=alpha*B`, depending on `TransA`.

In either case, the results overwrite the values of matrix `B` in `X`.

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

func cblas_srotmg(UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, Float, UnsafeMutablePointer&lt;Float>)

Generates a modified Givens rotation matrix.

func cblas_ssbmv(CBLAS_ORDER, CBLAS_UPLO, __LAPACK_int, __LAPACK_int, Float, UnsafePointer&lt;Float>?, __LAPACK_int, UnsafePointer&lt;Float>?, __LAPACK_int, Float, UnsafeMutablePointer&lt;Float>?, __LAPACK_int)

Scales a symmetric band matrix, then multiplies by a vector, then adds a vector (single-precision).

func cblas_sscal(__LAPACK_int, Float, UnsafeMutablePointer&lt;Float>?, __LAPACK_int)

Multiplies each element of a vector by a constant (single-precision).

func cblas_sspmv(CBLAS_ORDER, CBLAS_UPLO, __LAPACK_int, Float, UnsafePointer&lt;Float>?, UnsafePointer&lt;Float>?, __LAPACK_int, Float, UnsafeMutablePointer&lt;Float>?, __LAPACK_int)

Scales a packed symmetric matrix, then multiplies by a vector, then scales and adds another vector (single precision).

