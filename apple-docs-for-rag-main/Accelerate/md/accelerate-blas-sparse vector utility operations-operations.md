

- Accelerate
- BLAS
-  Sparse Vector Utility Operations 

API Collection

# Sparse Vector Utility Operations

Create and work with sparse vector structures.

## Topics

### Sparse Utility Operations

func sparse_get_vector_nonzero_count_double(sparse_dimension, UnsafePointer&lt;Double>!, sparse_stride) -> Int

Returns the number of nonzero values in the double-precision dense vector *x*.

func sparse_get_vector_nonzero_count_float(sparse_dimension, UnsafePointer&lt;Float>!, sparse_stride) -> Int

Returns the number of nonzero values in the single-precision dense vector *x*.

func sparse_pack_vector_double(sparse_dimension, sparse_dimension, UnsafePointer&lt;Double>!, sparse_stride, UnsafeMutablePointer&lt;Double>!, UnsafeMutablePointer&lt;sparse_index>!) -> Int

Packs nonzero values from a double-precision dense vector to a destination array.

func sparse_pack_vector_float(sparse_dimension, sparse_dimension, UnsafePointer&lt;Float>!, sparse_stride, UnsafeMutablePointer&lt;Float>!, UnsafeMutablePointer&lt;sparse_index>!) -> Int

Packs nonzero values from a single-precision dense vector to a destination array.

func sparse_unpack_vector_double(sparse_dimension, sparse_dimension, Bool, UnsafePointer&lt;Double>!, UnsafePointer&lt;sparse_index>!, UnsafeMutablePointer&lt;Double>!, sparse_stride)

Extracts elements from the sparse vector *x* into the corresponding location in the dense vector *y*, with both vectors containing double-precision values.

func sparse_unpack_vector_float(sparse_dimension, sparse_dimension, Bool, UnsafePointer&lt;Float>!, UnsafePointer&lt;sparse_index>!, UnsafeMutablePointer&lt;Float>!, sparse_stride)

Extracts elements from the sparse vector *x* into the corresponding location in the dense vector *y*, with both vectors containing single-precision values.

### Supporting Types

typealias sparse_dimension

The dimension type.

typealias sparse_index

The index type.

typealias sparse_stride

The stride type.

## See Also

### Sparse computation

Matrix and Vector Operations

Perform computations with matrices and vectors.

Pointwise Matrix Operations

Create, insert values into, and extract values from a pointwise sparse matrix.

Blockwise Matrix Operations

Create, insert values into, and extract values from a blockwise sparse matrix.

General Sparse Matrix Management Operations

Manage and work with the properties of a sparse matrix.

