

- Accelerate
-  appleblas_sgeadd(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# appleblas_sgeadd(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func appleblas_sgeadd(
    _ ORDER: CBLAS_ORDER,
    _ TRANSA: CBLAS_TRANSPOSE,
    _ TRANSB: CBLAS_TRANSPOSE,
    _ M: __LAPACK_int,
    _ N: __LAPACK_int,
    _ ALPHA: Float,
    _ A: UnsafePointer?,
    _ LDA: __LAPACK_int,
    _ BETA: Float,
    _ B: UnsafePointer?,
    _ LDB: __LAPACK_int,
    _ C: UnsafeMutablePointer,
    _ LDC: __LAPACK_int
)
```

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

