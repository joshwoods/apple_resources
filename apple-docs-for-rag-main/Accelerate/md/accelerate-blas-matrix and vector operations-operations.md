

- Accelerate
- BLAS
-  Matrix and Vector Operations 

API Collection

# Matrix and Vector Operations

Perform computations with matrices and vectors.

## Topics

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

func sparse_matrix_triangular_solve_dense_float(CBLAS_ORDER, CBLAS_TRANSPOSE, sparse_dimension, Float, sparse_matrix_float!, UnsafeMutablePointer&lt;Float>!, sparse_dimension) -> sparse_status

Solves the system of equations *B = alpha \* T⁻¹ \* B* for *B* where *B* is a dense matrix and *T* is a triangular sparse matrix, both with double-precision values.

### Matrix-Vector Operations

func sparse_matrix_vector_product_dense_double(CBLAS_TRANSPOSE, Double, sparse_matrix_double!, UnsafePointer&lt;Double>!, sparse_stride, UnsafeMutablePointer&lt;Double>!, sparse_stride) -> sparse_status

Multiplies the dense vector *x* by the sparse matrix *A* and adds the result to the dense vector *y*, with all operands containing double-precision values.

func sparse_matrix_vector_product_dense_float(CBLAS_TRANSPOSE, Float, sparse_matrix_float!, UnsafePointer&lt;Float>!, sparse_stride, UnsafeMutablePointer&lt;Float>!, sparse_stride) -> sparse_status

Multiplies the dense vector *x* by the sparse matrix *A* and adds the result to the dense vector *y*, with all operands containing single-precision values.

func sparse_vector_triangular_solve_dense_double(CBLAS_TRANSPOSE, Double, sparse_matrix_double!, UnsafeMutablePointer&lt;Double>!, sparse_stride) -> sparse_status

Solves the system of equations *x = alpha \* T⁻¹ \* x* for x where *x* is a dense vector and *T* is a triangular sparse matrix, with all operands containing double-precision values.

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

### Vector-Vector Operations

func sparse_inner_product_dense_double(sparse_dimension, UnsafePointer&lt;Double>!, UnsafePointer&lt;sparse_index>!, UnsafePointer&lt;Double>!, sparse_stride) -> Double

Computes the inner product of sparse vector *x* with double-precision *y*, with both vectors containing double-precision values.

func sparse_inner_product_dense_float(sparse_dimension, UnsafePointer&lt;Float>!, UnsafePointer&lt;sparse_index>!, UnsafePointer&lt;Float>!, sparse_stride) -> Float

Computes the inner product of sparse vector *x* with dense vector *y,* with both vectors containing single-precision values.

func sparse_inner_product_sparse_double(sparse_dimension, sparse_dimension, UnsafePointer&lt;Double>!, UnsafePointer&lt;sparse_index>!, UnsafePointer&lt;Double>!, UnsafePointer&lt;sparse_index>!) -> Double

Computes the inner product of sparse vector *x* with sparse vector *y,* with both vectors containing double-precision values.

func sparse_inner_product_sparse_float(sparse_dimension, sparse_dimension, UnsafePointer&lt;Float>!, UnsafePointer&lt;sparse_index>!, UnsafePointer&lt;Float>!, UnsafePointer&lt;sparse_index>!) -> Float

Computes the inner product of sparse vector *x* with sparse vector *y,* with both vectors containing single-precision values.

func sparse_vector_add_with_scale_dense_double(sparse_dimension, Double, UnsafePointer&lt;Double>!, UnsafePointer&lt;sparse_index>!, UnsafeMutablePointer&lt;Double>!, sparse_stride)

Scales the sparse vector *x* by *alpha* and adds the result to the dense vector *y,* with both vectors containing double-precision values.

func sparse_vector_add_with_scale_dense_float(sparse_dimension, Float, UnsafePointer&lt;Float>!, UnsafePointer&lt;sparse_index>!, UnsafeMutablePointer&lt;Float>!, sparse_stride)

Scales the sparse vector *x* by *alpha* and adds the result to the dense vector *y,* with both vectors containing single-precision values.

func sparse_vector_norm_double(sparse_dimension, UnsafePointer&lt;Double>!, UnsafePointer&lt;sparse_index>!, sparse_norm) -> Double

Computes the specified norm of the double-precision sparse vector *x*.

func sparse_vector_norm_float(sparse_dimension, UnsafePointer&lt;Float>!, UnsafePointer&lt;sparse_index>!, sparse_norm) -> Float

Computes the specified norm of the single-precision sparse vector *x*.

### Supporting Types

typealias sparse_matrix_double

Sparse matrix opaque type for double.

typealias sparse_matrix_float

Sparse matrix opaque type for float.

struct sparse_status

The type reflecting the status of an operations.

typealias sparse_dimension

The dimension type.

typealias sparse_index

The index type.

struct sparse_norm

The norm specifier.

typealias sparse_stride

The stride type.

## See Also

### Sparse computation

Pointwise Matrix Operations

Create, insert values into, and extract values from a pointwise sparse matrix.

Blockwise Matrix Operations

Create, insert values into, and extract values from a blockwise sparse matrix.

General Sparse Matrix Management Operations

Manage and work with the properties of a sparse matrix.

Sparse Vector Utility Operations

Create and work with sparse vector structures.

