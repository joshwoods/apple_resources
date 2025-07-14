

- Accelerate
-  sparse_outer_product_dense_double(\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# sparse_outer_product_dense_double(\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Computes the outer product of the dense vector *x* and the sparse vector *y*, with both operands containing double-precision values.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func sparse_outer_product_dense_double(
    _ M: sparse_dimension,
    _ N: sparse_dimension,
    _ nz: sparse_dimension,
    _ alpha: Double,
    _ x: UnsafePointer!,
    _ incx: sparse_stride,
    _ y: UnsafePointer!,
    _ indy: UnsafePointer!,
    _ C: UnsafeMutablePointer!
) -> sparse_status
```

## Parameters 

`M`  

The number of rows of *x* and the resulting matrix.

`N`  

The number of columns of the resulting matrix. The number of nonzero values must be less than or equal to `N`.

`nz`  

The number of nonzero values in the sparse vector *y*. Must be less than or equal to `N`.

`alpha`  

Scalar multiplier of *x*.

`x`  

Pointer to the dense vector *x*. Must be `M` number of elements. Negative strides are supported. Note, unlike dense BLAS routines, the pointer points to the last element when stride is negative.

`incx`  

Increment between valid values in the dense vector *x*. Negative strides are supported.

`y`  

Pointer to the dense storage for the values of the sparse vector *y*. The corresponding entry in `indy` holds the index of the value. Contains `nz` values.

`indy`  

Pointer to the dense storage for the index values of the sparse vector y. The corresponding entry in *y* holds the values of the vector. Contains `nz` values.

`C`  

Pointer to an uninitialized sparse matrix object. On success a newly allocated sparse matrix object is returned in this pointer. On error, this set to `NULL`.You are responsible for calling sparse_matrix_destroy(_:) on this matrix object.

## Return Value

On success SPARSE_SUCCESS is returned an `C` is valid matrix object. The caller is responsible for cleaning up the sparse matrix object with sparse_matrix_destroy(_:).

## Discussion

Will return SPARSE_ILLEGAL_PARAMETER if `nz > N`, and `C` will be unchanged.

## Discussion

Compute the outer product of the dense vector x and the sparse vector y and return a new sparse matrix in the uninitialized pointer sparse matrix pointer `C`. `C = alpha * x * y'`. You are responsible for calling sparse_matrix_destroy(_:) on the returned matrix.The matrix object returned on success is a point wise based sparse matrix.

Indices in `indx` are always assumed to be stored in ascending order. Additionally, indices are assumed to be unique. The behavior of this function is undefined if either of these assumptions are not met.

All indices are 0 based (the first element of a pointer is `ptr[0]`).

Important

Apple provides the BLAS and LAPACK libraries under the Accelerate framework to be in line with LAPACK 3.9.1. Starting with iOS 18, iPadOS 18, macOS 15, tvOS 18, watchOS 18, and visionOS 2, the libraries are in line with LAPACK 3.11.0. These new interfaces provide additional functionality, as well as a new ILP64 interface. To use the new interfaces, define `ACCELERATE_NEW_LAPACK` before including the Accelerate or vecLib headers. For ILP64 interfaces, also define `ACCELERATE_LAPACK_ILP64`. For Swift projects, specify `ACCELERATE_NEW_LAPACK=1` and `ACCELERATE_LAPACK_ILP64=1` as preprocessor macros in Xcode build settings.

## See Also

### Matrix-Vector Operations

func sparse_matrix_vector_product_dense_double(CBLAS_TRANSPOSE, Double, sparse_matrix_double!, UnsafePointer&lt;Double>!, sparse_stride, UnsafeMutablePointer&lt;Double>!, sparse_stride) -> sparse_status

Multiplies the dense vector *x* by the sparse matrix *A* and adds the result to the dense vector *y*, with all operands containing double-precision values.

func sparse_matrix_vector_product_dense_float(CBLAS_TRANSPOSE, Float, sparse_matrix_float!, UnsafePointer&lt;Float>!, sparse_stride, UnsafeMutablePointer&lt;Float>!, sparse_stride) -> sparse_status

Multiplies the dense vector *x* by the sparse matrix *A* and adds the result to the dense vector *y*, with all operands containing single-precision values.

func sparse_vector_triangular_solve_dense_double(CBLAS_TRANSPOSE, Double, sparse_matrix_double!, UnsafeMutablePointer&lt;Double>!, sparse_stride) -> sparse_status

Solves the system of equations *x = alpha \* T⁻¹ \* x* for x where *x* is a dense vector and *T* is a triangular sparse matrix, with all operands containing double-precision values.

func sparse_vector_triangular_solve_dense_float(CBLAS_TRANSPOSE, Float, sparse_matrix_float!, UnsafeMutablePointer&lt;Float>!, sparse_stride) -> sparse_status

Solves the system of equations *x = alpha \* T⁻¹ \* x* for x where *x* is a dense vector and *T* is a triangular sparse matrix, with all operands containing single-precision values.

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

