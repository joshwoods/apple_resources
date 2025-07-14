

- Accelerate
-  cblas_ztbmv(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# cblas_ztbmv(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Scales a triangular band matrix, then multiplies by a vector (double-precision complex).

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func cblas_ztbmv(
    _ ORDER: CBLAS_ORDER,
    _ UPLO: CBLAS_UPLO,
    _ TRANSA: CBLAS_TRANSPOSE,
    _ DIAG: CBLAS_DIAG,
    _ N: __LAPACK_int,
    _ K: __LAPACK_int,
    _ A: OpaquePointer?,
    _ LDA: __LAPACK_int,
    _ X: OpaquePointer?,
    _ INCX: __LAPACK_int
)
```

## Parameters 

`ORDER`  

Specifies row-major (C) or column-major (Fortran) data ordering.

`UPLO`  

Specifies whether to use the upper or lower triangle from the matrix. Valid values are `'U'` or `'L'`.

`TRANSA`  

Specifies whether to use matrix A (`'N'` or `'n'`) or the transpose of A (`'T'`, `'t'`, `'C'`, or `'c'`).

`DIAG`  

Specifies whether the matrix is unit triangular. Possible values are `'U'` (unit triangular) or `'N'` (not unit triangular).

`N`  

The order of matrix `A`.

`K`  

Half-bandwidth of matrix `A`.

`A`  

Matrix `A`.

`LDA`  

The leading dimension of array containing matrix `A`.

`X`  

Vector `x`.

`INCX`  

Stride within `X`. For example, if `incX` is 7, every 7th element is used.

## Discussion

Computes `A*x` and stores the results in `x`.

Important

Apple provides the BLAS and LAPACK libraries under the Accelerate framework to be in line with LAPACK 3.9.1. Starting with iOS 18, iPadOS 18, macOS 15, tvOS 18, watchOS 18, and visionOS 2, the libraries are in line with LAPACK 3.11.0. These new interfaces provide additional functionality, as well as a new ILP64 interface. To use the new interfaces, define `ACCELERATE_NEW_LAPACK` before including the Accelerate or vecLib headers. For ILP64 interfaces, also define `ACCELERATE_LAPACK_ILP64`. For Swift projects, specify `ACCELERATE_NEW_LAPACK=1` and `ACCELERATE_LAPACK_ILP64=1` as preprocessor macros in Xcode build settings.

## See Also

### Double-precision complex matrix functions

func cblas_dzasum(__LAPACK_int, OpaquePointer?, __LAPACK_int) -> Double

Computes the sum of the absolute values of real and imaginary parts of elements in a vector (single-precision complex).

func cblas_dznrm2(__LAPACK_int, OpaquePointer?, __LAPACK_int) -> Double

Computes the unitary norm of a vector (double-precision complex).

func cblas_zaxpy(__LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int)

Computes a constant times a vector plus a vector (double-precision complex).

func cblas_zcopy(__LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int)

Copies a vector to another vector (double-precision complex).

func cblas_zdrot(__LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, Double, Double)

Applies a Givens rotation matrix to a pair of complex vectors.

func cblas_zdscal(__LAPACK_int, Double, OpaquePointer?, __LAPACK_int)

Multiplies each element of a vector by a constant (double-precision complex).

func cblas_zgbmv(CBLAS_ORDER, CBLAS_TRANSPOSE, __LAPACK_int, __LAPACK_int, __LAPACK_int, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int)

Scales a general band matrix, then multiplies by a vector, then adds a vector (double-precision complex).

func cblas_zgemm(CBLAS_ORDER, CBLAS_TRANSPOSE, CBLAS_TRANSPOSE, __LAPACK_int, __LAPACK_int, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int)

Multiplies two matrices (double-precision complex).

func cblas_zgemv(CBLAS_ORDER, CBLAS_TRANSPOSE, __LAPACK_int, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int)

Multiplies a matrix by a vector (double-precision complex).

func cblas_zgerc(CBLAS_ORDER, __LAPACK_int, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int)

Multiplies vector X by the conjugate transpose of vector Y, then adds matrix A (double-precision complex).

func cblas_zgeru(CBLAS_ORDER, __LAPACK_int, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int)

Multiplies vector X by the transpose of vector Y, then adds matrix A (double-precision complex).

func cblas_zhbmv(CBLAS_ORDER, CBLAS_UPLO, __LAPACK_int, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int)

Scales a Hermitian band matrix, then multiplies by a vector, then adds a vector (double-precision complex).

func cblas_zhemm(CBLAS_ORDER, CBLAS_SIDE, CBLAS_UPLO, __LAPACK_int, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int)

Multiplies two Hermitian matrices (double-precision complex).

func cblas_zhemv(CBLAS_ORDER, CBLAS_UPLO, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int)

Scales and multiplies a Hermitian matrix by a vector, then adds a second (scaled) vector.

func cblas_zher(CBLAS_ORDER, CBLAS_UPLO, __LAPACK_int, Double, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int)

Adds the product of a scaling factor, vector `X`, and the conjugate transpose of `X` to matrix `A`.

