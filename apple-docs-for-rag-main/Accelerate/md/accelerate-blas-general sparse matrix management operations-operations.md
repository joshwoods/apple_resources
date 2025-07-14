

- Accelerate
- BLAS
-  General Sparse Matrix Management Operations 

API Collection

# General Sparse Matrix Management Operations

Manage and work with the properties of a sparse matrix.

## Topics

### General Sparse Matrix Management Operations

func sparse_commit(UnsafeMutableRawPointer!) -> sparse_status

Puts values that you recently added to the matrix into the internal sparse storage format.

func sparse_matrix_destroy(UnsafeMutableRawPointer!) -> sparse_status

Releases any memory associated with the matrix object.

func sparse_set_matrix_property(UnsafeMutableRawPointer!, sparse_matrix_property) -> sparse_status

Sets the given property for a matrix object.

func sparse_get_matrix_property(UnsafeMutableRawPointer!, sparse_matrix_property) -> Int

Returns the value of the given property name.

func sparse_get_matrix_number_of_rows(UnsafeMutableRawPointer!) -> sparse_dimension

Returns the number of rows of a matrix.

func sparse_get_matrix_number_of_columns(UnsafeMutableRawPointer!) -> sparse_dimension

Returns the number of columns of a matrix.

func sparse_get_matrix_nonzero_count(UnsafeMutableRawPointer!) -> Int

Returns the number of nonzero values of a matrix.

func sparse_get_matrix_nonzero_count_for_row(UnsafeMutableRawPointer!, sparse_index) -> Int

Returns the number of nonzero values in a row of a matrix.

func sparse_get_matrix_nonzero_count_for_column(UnsafeMutableRawPointer!, sparse_index) -> Int

Returns the number of nonzero values in a column of a matrix.

### Supporting Types

typealias sparse_dimension

The dimension type.

typealias sparse_index

The index type.

struct sparse_matrix_property

The matrix property type.

## See Also

### Sparse computation

Matrix and Vector Operations

Perform computations with matrices and vectors.

Pointwise Matrix Operations

Create, insert values into, and extract values from a pointwise sparse matrix.

Blockwise Matrix Operations

Create, insert values into, and extract values from a blockwise sparse matrix.

Sparse Vector Utility Operations

Create and work with sparse vector structures.

