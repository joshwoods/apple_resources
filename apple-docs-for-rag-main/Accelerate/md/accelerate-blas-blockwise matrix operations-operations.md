

- Accelerate
- BLAS
-  Blockwise Matrix Operations 

API Collection

# Blockwise Matrix Operations

Create, insert values into, and extract values from a blockwise sparse matrix.

## Topics

### Matrix Creation and Population

func sparse_matrix_block_create_double(sparse_dimension, sparse_dimension, sparse_dimension, sparse_dimension) -> sparse_matrix_double!

Returns a double-precision sparse matrix object that is stored in block-entry format with a fixed block size.

func sparse_matrix_block_create_float(sparse_dimension, sparse_dimension, sparse_dimension, sparse_dimension) -> sparse_matrix_float!

Returns a single-precision sparse matrix object that is stored in block-entry format with a fixed block size.

func sparse_matrix_variable_block_create_double(sparse_dimension, sparse_dimension, UnsafePointer&lt;sparse_dimension>!, UnsafePointer&lt;sparse_dimension>!) -> sparse_matrix_double!

Returns a double-precision sparse matrix object that is stored in block-entry format with a variable block size.

func sparse_matrix_variable_block_create_float(sparse_dimension, sparse_dimension, UnsafePointer&lt;sparse_dimension>!, UnsafePointer&lt;sparse_dimension>!) -> sparse_matrix_float!

Returns a single-precision sparse matrix object that is stored in block-entry format with a variable block size.

func sparse_insert_block_double(sparse_matrix_double!, UnsafePointer&lt;Double>!, sparse_dimension, sparse_dimension, sparse_index, sparse_index) -> sparse_status

Inserts a dense block of entries into a double-precision matrix.

func sparse_insert_block_float(sparse_matrix_float!, UnsafePointer&lt;Float>!, sparse_dimension, sparse_dimension, sparse_index, sparse_index) -> sparse_status

Inserts a dense block of entries into a single-precision matrix.

### Value Extraction

func sparse_extract_block_double(sparse_matrix_double!, sparse_index, sparse_index, sparse_dimension, sparse_dimension, UnsafeMutablePointer&lt;Double>!) -> sparse_status

Extracts values from a specified block of a double-precision matrix.

func sparse_extract_block_float(sparse_matrix_float!, sparse_index, sparse_index, sparse_dimension, sparse_dimension, UnsafeMutablePointer&lt;Float>!) -> sparse_status

Extracts values from a specified block of a single-precision matrix.

### Block Dimension Queries

func sparse_get_block_dimension_for_row(UnsafeMutableRawPointer!, sparse_index) -> Int

Returns the dimension of the block for a specified row of a double-precision matrix.

func sparse_get_block_dimension_for_col(UnsafeMutableRawPointer!, sparse_index) -> Int

Returns the dimension of the block for a specified column of a single-precision matrix.

### Supporting Types

typealias sparse_dimension

The dimension type.

typealias sparse_index

The index type.

typealias sparse_matrix_double

Sparse matrix opaque type for double.

typealias sparse_matrix_float

Sparse matrix opaque type for float.

struct sparse_status

The type reflecting the status of an operations.

## See Also

### Sparse computation

Matrix and Vector Operations

Perform computations with matrices and vectors.

Pointwise Matrix Operations

Create, insert values into, and extract values from a pointwise sparse matrix.

General Sparse Matrix Management Operations

Manage and work with the properties of a sparse matrix.

Sparse Vector Utility Operations

Create and work with sparse vector structures.

