

- Accelerate
-  cblas_cgerc(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# cblas_cgerc(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Multiplies vector X by the conjugate transpose of vector Y, then adds matrix A (single-precision complex).

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func cblas_cgerc(
    _ ORDER: CBLAS_ORDER,
    _ M: __LAPACK_int,
    _ N: __LAPACK_int,
    _ ALPHA: OpaquePointer,
    _ X: OpaquePointer?,
    _ INCX: __LAPACK_int,
    _ Y: OpaquePointer?,
    _ INCY: __LAPACK_int,
    _ A: OpaquePointer?,
    _ LDA: __LAPACK_int
)
```

## Parameters 

`ORDER`  

Specifies row-major (C) or column-major (Fortran) data ordering.

`M`  

Number of rows in matrix `A`.

`N`  

Number of columns in matrix `A`.

`ALPHA`  

Scaling factor for vector `X`.

`X`  

Vector `X`.

`INCX`  

Stride within `X`. For example, if `incX` is 7, every 7th element is used.

`Y`  

Vector `Y`.

`INCY`  

Stride within `Y`. For example, if `incY` is 7, every 7th element is used.

`A`  

Matrix `A`.

`LDA`  

Leading dimension of array containing matrix `A`.

## Discussion

Computes `alpha*x*conjg(y') + A`.

Important

Apple provides the BLAS and LAPACK libraries under the Accelerate framework to be in line with LAPACK 3.9.1. Starting with iOS 18, iPadOS 18, macOS 15, tvOS 18, watchOS 18, and visionOS 2, the libraries are in line with LAPACK 3.11.0. These new interfaces provide additional functionality, as well as a new ILP64 interface. To use the new interfaces, define `ACCELERATE_NEW_LAPACK` before including the Accelerate or vecLib headers. For ILP64 interfaces, also define `ACCELERATE_LAPACK_ILP64`. For Swift projects, specify `ACCELERATE_NEW_LAPACK=1` and `ACCELERATE_LAPACK_ILP64=1` as preprocessor macros in Xcode build settings.

## See Also

### Single-precision complex matrix functions

func cblas_caxpy(__LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int)

Computes a constant times a vector plus a vector (single-precision complex).

func cblas_ccopy(__LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int)

Copies a vector to another vector (single-precision complex).

func cblas_cgbmv(CBLAS_ORDER, CBLAS_TRANSPOSE, __LAPACK_int, __LAPACK_int, __LAPACK_int, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int)

Scales a general band matrix, then multiplies by a vector, then adds a vector (single-precision complex).

func cblas_cgemm(CBLAS_ORDER, CBLAS_TRANSPOSE, CBLAS_TRANSPOSE, __LAPACK_int, __LAPACK_int, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int)

Multiplies two matrices (single-precision complex).

func cblas_cgemv(CBLAS_ORDER, CBLAS_TRANSPOSE, __LAPACK_int, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int)

Multiplies a matrix by a vector (single-precision complex).

func cblas_cgeru(CBLAS_ORDER, __LAPACK_int, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int)

Multiplies vector X by the transpose of vector Y, then adds matrix A (single-precision complex).

func cblas_chbmv(CBLAS_ORDER, CBLAS_UPLO, __LAPACK_int, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int)

Scales a Hermitian band matrix, then multiplies by a vector, then adds a vector (single-precision complex).

func cblas_chemm(CBLAS_ORDER, CBLAS_SIDE, CBLAS_UPLO, __LAPACK_int, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int)

Multiplies two Hermitian matrices (single-precision complex), then adds a third (with scaling).

func cblas_chemv(CBLAS_ORDER, CBLAS_UPLO, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int)

Scales and multiplies a Hermitian matrix by a vector, then adds a second (scaled) vector.

func cblas_cher(CBLAS_ORDER, CBLAS_UPLO, __LAPACK_int, Float, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int)

Hermitian rank 1 update: adds the product of a scaling factor, vector `X`, and the conjugate transpose of `X` to matrix `A`.

func cblas_cher2(CBLAS_ORDER, CBLAS_UPLO, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int)

Hermitian rank 2 update: adds the product of a scaling factor, vector `X`, and the conjugate transpose of vector `Y` to the product of the conjugate of the scaling factor, vector `Y`, and the conjugate transpose of vector `X`, and adds the result to matrix `A`.

func cblas_cher2k(CBLAS_ORDER, CBLAS_UPLO, CBLAS_TRANSPOSE, __LAPACK_int, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int, OpaquePointer?, __LAPACK_int, Float, OpaquePointer?, __LAPACK_int)

Performs a rank-2k update of a complex Hermitian matrix (single-precision complex).

func cblas_cherk(CBLAS_ORDER, CBLAS_UPLO, CBLAS_TRANSPOSE, __LAPACK_int, __LAPACK_int, Float, OpaquePointer?, __LAPACK_int, Float, OpaquePointer?, __LAPACK_int)

Rank-k update—multiplies a Hermitian matrix by its transpose and adds a second matrix (single precision).

func cblas_chpmv(CBLAS_ORDER, CBLAS_UPLO, __LAPACK_int, OpaquePointer, OpaquePointer?, OpaquePointer?, __LAPACK_int, OpaquePointer, OpaquePointer?, __LAPACK_int)

Scales a packed hermitian matrix, multiplies it by a vector, and adds a scaled vector.

func cblas_chpr(CBLAS_ORDER, CBLAS_UPLO, __LAPACK_int, Float, OpaquePointer?, __LAPACK_int, OpaquePointer?)

Scales and multiplies a vector times its conjugate transpose, then adds a matrix.

