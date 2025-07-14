

- Accelerate
-  sparse_matrix_triangular_solve_dense_float(\_:\_:\_:\_:\_:\_:\_:) 

Function

# sparse_matrix_triangular_solve_dense_float(\_:\_:\_:\_:\_:\_:\_:)

Solves the system of equations *B = alpha \* T⁻¹ \* B* for *B* where *B* is a dense matrix and *T* is a triangular sparse matrix, both with double-precision values.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func sparse_matrix_triangular_solve_dense_float(
    _ order: CBLAS_ORDER,
    _ transt: CBLAS_TRANSPOSE,
    _ nrhs: sparse_dimension,
    _ alpha: Float,
    _ T: sparse_matrix_float!,
    _ B: UnsafeMutablePointer!,
    _ ldb: sparse_dimension
) -> sparse_status
```

## Parameters 

`order`  

Specified the storage order for the dense matrix *B*. Must be one of `CblasRowMajor` or `CblasColMajor`.

`transt`  

Specifies whether to perform the operation with *T* or the transpose of *T*. Must be one of `CblasNoTrans` or `CblasTrans`.

`nrhs`  

The number of columns of the matrix *B*.

`alpha`  

Scalar multiplier of *T*.

`T`  

The sparse triangular matrix, *T*. Must be upper or lower triangular matrix. Will return SPARSE_ILLEGAL_PARAMETER if not a triangular matrix.

`B`  

Pointer to the dense matrix *B*. The number of rows must be equal to the number of columns of *T* and the number of columns is `nrhs`. Behavior undefined if this is not met. The argument `ldb` describes how many elements to move between one row (row major) or column (column major). On exit holds the solution to the system of equations.

`ldb`  

Increment in elements between rows (row major) or columns (column major) of *B*. Must be greater than or equal to `nrhs` when row major, or number of columns of *A* when column major.

## Return Value

On success, SPARSE_SUCCESS is returned and *B* has been updated with result of the operation. Will return SPARSE_ILLEGAL_PARAMETER if either of order or `transt` are invalid or the `ldb` does not meet its dimension requirements. On error, *B* is unchanged.

## Discussion

If *T* is of size *N x N*, then *B* must be of size *N x* `nrhs`. The matrix *T* must be an upper or lower triangular matrix.

Important

Apple provides the BLAS and LAPACK libraries under the Accelerate framework to be in line with LAPACK 3.9.1. Starting with iOS 18, iPadOS 18, macOS 15, tvOS 18, watchOS 18, and visionOS 2, the libraries are in line with LAPACK 3.11.0. These new interfaces provide additional functionality, as well as a new ILP64 interface. To use the new interfaces, define `ACCELERATE_NEW_LAPACK` before including the Accelerate or vecLib headers. For ILP64 interfaces, also define `ACCELERATE_LAPACK_ILP64`. For Swift projects, specify `ACCELERATE_NEW_LAPACK=1` and `ACCELERATE_LAPACK_ILP64=1` as preprocessor macros in Xcode build settings.

## See Also

### Matrix-Matrix Operations

func sparse_matrix_product_dense_double(CBLAS_ORDER, CBLAS_TRANSPOSE, sparse_dimension, Double, sparse_matrix_double!, UnsafePointer&lt;Double>!, sparse_dimension, UnsafeMutablePointer&lt;Double>!, sparse_dimension) -> sparse_status

Multiplies the dense matrix *B* by the sparse matrix *A* and adds the result to the dense matrix *C*, all with double-precision values.

func sparse_matrix_product_dense_float(CBLAS_ORDER, CBLAS_TRANSPOSE, sparse_dimension, Float, sparse_matrix_float!, UnsafePointer&lt;Float>!, sparse_dimension, UnsafeMutablePointer&lt;Float>!, sparse_dimension) -> sparse_status

Multiplies the dense matrix *B* by the sparse matrix *A* and adds the result to the dense matrix *C*, all with single-precision values.

func sparse_matrix_product_sparse_double(CBLAS_ORDER, CBLAS_TRANSPOSE, Double, sparse_matrix_double!, sparse_matrix_double!, UnsafeMutablePointer&lt;Double>!, sparse_dimension) -> sparse_status

Multiplies the sparse matrix *B* by the sparse matrix *A* and adds the result to the dense matrix *C*, all with double-precision values.

func sparse_matrix_product_sparse_float(CBLAS_ORDER, CBLAS_TRANSPOSE, Float, sparse_matrix_float!, sparse_matrix_float!, UnsafeMutablePointer&lt;Float>!, sparse_dimension) -> sparse_status

Multiplies the sparse matrix *B* by the sparse matrix *A* and adds the result to the dense matrix *C*, all with single-precision values.

func sparse_matrix_triangular_solve_dense_double(CBLAS_ORDER, CBLAS_TRANSPOSE, sparse_dimension, Double, sparse_matrix_double!, UnsafeMutablePointer&lt;Double>!, sparse_dimension) -> sparse_status

Solves the system of equations *B = alpha \* T⁻¹ \* B* for *B* where *B* is a dense matrix and *T* is a triangular sparse matrix, both with double-precision values.

