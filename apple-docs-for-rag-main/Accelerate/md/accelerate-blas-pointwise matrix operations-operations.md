

- Accelerate
- BLAS
-  Pointwise Matrix Operations 

API Collection

# Pointwise Matrix Operations

Create, insert values into, and extract values from a pointwise sparse matrix.

## Topics

### Matrix Creation and Population

func sparse_matrix_create_double(sparse_dimension, sparse_dimension) -> sparse_matrix_double!

Returns a double-precision sparse matrix object.

func sparse_matrix_create_float(sparse_dimension, sparse_dimension) -> sparse_matrix_float!

Returns a single-precision sparse matrix object.

func sparse_insert_entry_double(sparse_matrix_double!, Double, sparse_index, sparse_index) -> sparse_status

Inserts a single scalar entry into a double-precision sparse matrix.

func sparse_insert_entry_float(sparse_matrix_float!, Float, sparse_index, sparse_index) -> sparse_status

Inserts a single scalar entry into a single-precision sparse matrix.

func sparse_insert_entries_double(sparse_matrix_double!, sparse_dimension, UnsafePointer&lt;Double>!, UnsafePointer&lt;sparse_index>!, UnsafePointer&lt;sparse_index>!) -> sparse_status

Inserts a list of scalar entries into a double-precision sparse matrix.

func sparse_insert_entries_float(sparse_matrix_float!, sparse_dimension, UnsafePointer&lt;Float>!, UnsafePointer&lt;sparse_index>!, UnsafePointer&lt;sparse_index>!) -> sparse_status

Inserts a list of scalar entries into a single-precision sparse matrix.

func sparse_insert_col_double(sparse_matrix_double!, sparse_index, sparse_dimension, UnsafePointer&lt;Double>!, UnsafePointer&lt;sparse_index>!) -> sparse_status

Inserts a list of scalar entries into a single column of a double-precision sparse matrix.

func sparse_insert_col_float(sparse_matrix_float!, sparse_index, sparse_dimension, UnsafePointer&lt;Float>!, UnsafePointer&lt;sparse_index>!) -> sparse_status

Inserts a list of scalar entries into a single column of a single-precision sparse matrix.

func sparse_insert_row_double(sparse_matrix_double!, sparse_index, sparse_dimension, UnsafePointer&lt;Double>!, UnsafePointer&lt;sparse_index>!) -> sparse_status

Inserts a list of scalar entries into a single row of a double-precision sparse matrix.

func sparse_insert_row_float(sparse_matrix_float!, sparse_index, sparse_dimension, UnsafePointer&lt;Float>!, UnsafePointer&lt;sparse_index>!) -> sparse_status

Inserts a list of scalar entries into a single row of a single-precision sparse matrix.

### Value Extraction

func sparse_extract_sparse_row_double(sparse_matrix_double!, sparse_index, sparse_index, UnsafeMutablePointer&lt;sparse_index>!, sparse_dimension, UnsafeMutablePointer&lt;Double>!, UnsafeMutablePointer&lt;sparse_index>!) -> sparse_status

Extracts values from a specified row of a double-precision sparse matrix.

func sparse_extract_sparse_row_float(sparse_matrix_float!, sparse_index, sparse_index, UnsafeMutablePointer&lt;sparse_index>!, sparse_dimension, UnsafeMutablePointer&lt;Float>!, UnsafeMutablePointer&lt;sparse_index>!) -> sparse_status

Extracts values from a specified row of a single-precision sparse matrix.

func sparse_extract_sparse_column_double(sparse_matrix_double!, sparse_index, sparse_index, UnsafeMutablePointer&lt;sparse_index>!, sparse_dimension, UnsafeMutablePointer&lt;Double>!, UnsafeMutablePointer&lt;sparse_index>!) -> sparse_status

Extracts values from a specified column of a double-precision sparse matrix.

func sparse_extract_sparse_column_float(sparse_matrix_float!, sparse_index, sparse_index, UnsafeMutablePointer&lt;sparse_index>!, sparse_dimension, UnsafeMutablePointer&lt;Float>!, UnsafeMutablePointer&lt;sparse_index>!) -> sparse_status

Extracts values from a specified column of a single-precision sparse matrix.

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

Blockwise Matrix Operations

Create, insert values into, and extract values from a blockwise sparse matrix.

General Sparse Matrix Management Operations

Manage and work with the properties of a sparse matrix.

Sparse Vector Utility Operations

Create and work with sparse vector structures.

