

- Accelerate
-  sparse_matrix_create_double(\_:\_:) 

Function

# sparse_matrix_create_double(\_:\_:)

Returns a double-precision sparse matrix object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func sparse_matrix_create_double(
    _ M: sparse_dimension,
    _ N: sparse_dimension
) -> sparse_matrix_double!
```

## Parameters 

`M`  

The number of rows of the matrix. Must be greater than 0.

`N`  

The number of columns of the matrix. Must be greater than 0.

## Return Value

A matrix object that is ready for receiving entries. If an error occurs, `nil` is returned.

## Discussion

This function creates a sparse matrix object that is stored in pointwise format and is ready to receive values from the various insert routines. Pointwise format means individual values are stored for a given `i,j` location as opposed to blocks of values. For block support use the block create routines. See the various insert routines for details on inserting entries into this matrix object.

After you’ve finished with the matrix, it’s important that you free the memory allocated to it with sparse_matrix_destroy(_:).

Important

Apple provides the BLAS and LAPACK libraries under the Accelerate framework to be in line with LAPACK 3.9.1. Starting with iOS 18, iPadOS 18, macOS 15, tvOS 18, watchOS 18, and visionOS 2, the libraries are in line with LAPACK 3.11.0. These new interfaces provide additional functionality, as well as a new ILP64 interface. To use the new interfaces, define `ACCELERATE_NEW_LAPACK` before including the Accelerate or vecLib headers. For ILP64 interfaces, also define `ACCELERATE_LAPACK_ILP64`. For Swift projects, specify `ACCELERATE_NEW_LAPACK=1` and `ACCELERATE_LAPACK_ILP64=1` as preprocessor macros in Xcode build settings.

## See Also

### Matrix Creation and Population

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

