

- Accelerate
-  sparse_matrix_product_sparse_double(\_:\_:\_:\_:\_:\_:\_:) 

Function

# sparse_matrix_product_sparse_double(\_:\_:\_:\_:\_:\_:\_:)

Multiplies the sparse matrix *B* by the sparse matrix *A* and adds the result to the dense matrix *C*, all with double-precision values.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func sparse_matrix_product_sparse_double(
    _ order: CBLAS_ORDER,
    _ transa: CBLAS_TRANSPOSE,
    _ alpha: Double,
    _ A: sparse_matrix_double!,
    _ B: sparse_matrix_double!,
    _ C: UnsafeMutablePointer!,
    _ ldc: sparse_dimension
) -> sparse_status
```

## Parameters 

`order`  

The storage order for the dense matrix *C*. Must be one of `CblasRowMajor` or `CblasColMajor`.

`transa`  

Specifies whether to perform the operation with *A* or the transpose of *A*. Must be one of `CblasNoTrans` or `CblasTrans`.

`alpha`  

Scalar multiplier of *A*.

`A`  

The sparse matrix, *A*.

`B`  

The sparse matrix, B.

`C`  

Pointer to the dense matrix *C*. The number of rows must be equal to the number of rows of *A* and the number of columns must be equal to the number of columns of *B*. Behavior undefined if this is not met. The parameter `ldc` describes how many elements to move between one row (row major) or column (column major). *C* is updated with the result of the operation.

`ldc`  

Increment in elements between rows (row major) or columns (column major) of *C*. Must be greater than or equal to `B` when row major, or number of rows of *A* when column major.

## Return Value

On success, SPARSE_SUCCESS is returned and `C` has been updated with result of the operation. Will return SPARSE_ILLEGAL_PARAMETER if order or `transa` is not valid or the leading dimension parameters do not meet their dimension requirements. On error, `C` is unchanged.

## Discussion

Multiplies the sparse matrix *B* by the sparse matrix *A* and adds the result to the dense matrix *C* (*C = alpha \* op(A) \* B + C*, where *op(A)* is either *A* or the transpose of *A*). If *A* is of size *M x K*, then *B* is of size *K x N* and *C* is of size *M x N*.If the desired operation is *C = A \* B*, then an efficient option is to create the *C* buffer of zeros and then perform the operation with the zero filled *C*.

Important

Apple provides the BLAS and LAPACK libraries under the Accelerate framework to be in line with LAPACK 3.9.1. Starting with iOS 18, iPadOS 18, macOS 15, tvOS 18, watchOS 18, and visionOS 2, the libraries are in line with LAPACK 3.11.0. These new interfaces provide additional functionality, as well as a new ILP64 interface. To use the new interfaces, define `ACCELERATE_NEW_LAPACK` before including the Accelerate or vecLib headers. For ILP64 interfaces, also define `ACCELERATE_LAPACK_ILP64`. For Swift projects, specify `ACCELERATE_NEW_LAPACK=1` and `ACCELERATE_LAPACK_ILP64=1` as preprocessor macros in Xcode build settings.

## See Also

### Matrix-Matrix Operations

func sparse_matrix_product_dense_double(CBLAS_ORDER, CBLAS_TRANSPOSE, sparse_dimension, Double, sparse_matrix_double!, UnsafePointer&lt;Double>!, sparse_dimension, UnsafeMutablePointer&lt;Double>!, sparse_dimension) -> sparse_status

Multiplies the dense matrix *B* by the sparse matrix *A* and adds the result to the dense matrix *C*, all with double-precision values.

func sparse_matrix_product_dense_float(CBLAS_ORDER, CBLAS_TRANSPOSE, sparse_dimension, Float, sparse_matrix_float!, UnsafePointer&lt;Float>!, sparse_dimension, UnsafeMutablePointer&lt;Float>!, sparse_dimension) -> sparse_status

Multiplies the dense matrix *B* by the sparse matrix *A* and adds the result to the dense matrix *C*, all with single-precision values.

func sparse_matrix_product_sparse_float(CBLAS_ORDER, CBLAS_TRANSPOSE, Float, sparse_matrix_float!, sparse_matrix_float!, UnsafeMutablePointer&lt;Float>!, sparse_dimension) -> sparse_status

Multiplies the sparse matrix *B* by the sparse matrix *A* and adds the result to the dense matrix *C*, all with single-precision values.

func sparse_matrix_triangular_solve_dense_double(CBLAS_ORDER, CBLAS_TRANSPOSE, sparse_dimension, Double, sparse_matrix_double!, UnsafeMutablePointer&lt;Double>!, sparse_dimension) -> sparse_status

Solves the system of equations *B = alpha \* T⁻¹ \* B* for *B* where *B* is a dense matrix and *T* is a triangular sparse matrix, both with double-precision values.

func sparse_matrix_triangular_solve_dense_float(CBLAS_ORDER, CBLAS_TRANSPOSE, sparse_dimension, Float, sparse_matrix_float!, UnsafeMutablePointer&lt;Float>!, sparse_dimension) -> sparse_status

Solves the system of equations *B = alpha \* T⁻¹ \* B* for *B* where *B* is a dense matrix and *T* is a triangular sparse matrix, both with double-precision values.

