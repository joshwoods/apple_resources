

- Accelerate
-  sparse_vector_triangular_solve_dense_double(\_:\_:\_:\_:\_:) 

Function

# sparse_vector_triangular_solve_dense_double(\_:\_:\_:\_:\_:)

Solves the system of equations *x = alpha \* T⁻¹ \* x* for x where *x* is a dense vector and *T* is a triangular sparse matrix, with all operands containing double-precision values.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func sparse_vector_triangular_solve_dense_double(
    _ transt: CBLAS_TRANSPOSE,
    _ alpha: Double,
    _ T: sparse_matrix_double!,
    _ x: UnsafeMutablePointer!,
    _ incx: sparse_stride
) -> sparse_status
```

## Parameters 

`transt`  

Specifies whether to perform the operation with T or the transpose of T. Must be one of `CblasNoTrans` or `CblasTrans`.

`alpha`  

Scalar multiplier of *T*.

`T`  

The sparse triangular matrix. Must be upper or lower triangular matrix. Will return SPARSE_ILLEGAL_PARAMETER if not a triangular matrix.

`x`  

Pointer to the dense vector *x*. The dimension must match the dimension of the triangular matrix *T*. Behavior undefined if this is not met. Negative strides are supported. Note, unlike dense BLAS routines, the pointer points to the last element when stride is negative. On exit holds the solution to the system of equations.

`incx`  

Increment between valid values in the dense vector *x*. Negative strides are supported.

## Return Value

On success, SPARSE_SUCCESS (`x` will be updated with result of the operation). Will return SPARSE_ILLEGAL_PARAMETER if `transt` is invalid or if the matrix `T` is not triangular and `x` will be unchanged.

## Discussion

Important

Apple provides the BLAS and LAPACK libraries under the Accelerate framework to be in line with LAPACK 3.9.1. Starting with iOS 18, iPadOS 18, macOS 15, tvOS 18, watchOS 18, and visionOS 2, the libraries are in line with LAPACK 3.11.0. These new interfaces provide additional functionality, as well as a new ILP64 interface. To use the new interfaces, define `ACCELERATE_NEW_LAPACK` before including the Accelerate or vecLib headers. For ILP64 interfaces, also define `ACCELERATE_LAPACK_ILP64`. For Swift projects, specify `ACCELERATE_NEW_LAPACK=1` and `ACCELERATE_LAPACK_ILP64=1` as preprocessor macros in Xcode build settings.

## See Also

### Matrix-Vector Operations

func sparse_matrix_vector_product_dense_double(CBLAS_TRANSPOSE, Double, sparse_matrix_double!, UnsafePointer&lt;Double>!, sparse_stride, UnsafeMutablePointer&lt;Double>!, sparse_stride) -> sparse_status

Multiplies the dense vector *x* by the sparse matrix *A* and adds the result to the dense vector *y*, with all operands containing double-precision values.

func sparse_matrix_vector_product_dense_float(CBLAS_TRANSPOSE, Float, sparse_matrix_float!, UnsafePointer&lt;Float>!, sparse_stride, UnsafeMutablePointer&lt;Float>!, sparse_stride) -> sparse_status

Multiplies the dense vector *x* by the sparse matrix *A* and adds the result to the dense vector *y*, with all operands containing single-precision values.

func sparse_vector_triangular_solve_dense_float(CBLAS_TRANSPOSE, Float, sparse_matrix_float!, UnsafeMutablePointer&lt;Float>!, sparse_stride) -> sparse_status

Solves the system of equations *x = alpha \* T⁻¹ \* x* for x where *x* is a dense vector and *T* is a triangular sparse matrix, with all operands containing single-precision values.

func sparse_outer_product_dense_double(sparse_dimension, sparse_dimension, sparse_dimension, Double, UnsafePointer&lt;Double>!, sparse_stride, UnsafePointer&lt;Double>!, UnsafePointer&lt;sparse_index>!, UnsafeMutablePointer&lt;sparse_matrix_double?>!) -> sparse_status

Computes the outer product of the dense vector *x* and the sparse vector *y*, with both operands containing double-precision values.

func sparse_outer_product_dense_float(sparse_dimension, sparse_dimension, sparse_dimension, Float, UnsafePointer&lt;Float>!, sparse_stride, UnsafePointer&lt;Float>!, UnsafePointer&lt;sparse_index>!, UnsafeMutablePointer&lt;sparse_matrix_float?>!) -> sparse_status

Computes the outer product of the dense vector *x* and the sparse vector *y*, with both operands containing single-precision values.

func sparse_permute_rows_double(sparse_matrix_double!, UnsafePointer&lt;sparse_index>!) -> sparse_status

Permutes the rows of the double-precision sparse matrix *A* based on the provided permutation array.

func sparse_permute_rows_float(sparse_matrix_float!, UnsafePointer&lt;sparse_index>!) -> sparse_status

Permutes the rows of the single-precision sparse matrix *A* based on the provided permutation array.

func sparse_permute_cols_double(sparse_matrix_double!, UnsafePointer&lt;sparse_index>!) -> sparse_status

Permutes the columns of the double-precision sparse matrix *A* based on the provided permutation array.

func sparse_permute_cols_float(sparse_matrix_float!, UnsafePointer&lt;sparse_index>!) -> sparse_status

Permutes the columns of the single-precision sparse matrix *A* based on the provided permutation array.

func sparse_elementwise_norm_double(sparse_matrix_double!, sparse_norm) -> Double

Computes the specified element-wise norm of the double-precision sparse matrix *A*.

func sparse_elementwise_norm_float(sparse_matrix_float!, sparse_norm) -> Float

Computes the specified element-wise norm of the single-precision sparse matrix *A*.

func sparse_operator_norm_double(sparse_matrix_double!, sparse_norm) -> Double

Computes the specified operator norm of the double-precision sparse matrix *A*.

func sparse_operator_norm_float(sparse_matrix_float!, sparse_norm) -> Float

Computes the specified operator norm of the single-precision sparse matrix *A*.

func sparse_matrix_trace_double(sparse_matrix_double!, sparse_index) -> Double

Computes the sum along the specified diagonal of the double-precision sparse matrix *A*.

func sparse_matrix_trace_float(sparse_matrix_float!, sparse_index) -> Float

Computes the sum along the specified diagonal of the single-precision sparse matrix *A*.

