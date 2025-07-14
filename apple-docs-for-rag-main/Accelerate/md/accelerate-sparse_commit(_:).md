

- Accelerate
-  sparse_commit(\_:) 

Function

# sparse_commit(\_:)

Puts values that you recently added to the matrix into the internal sparse storage format.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func sparse_commit(_ A: UnsafeMutableRawPointer!) -> sparse_status
```

## Parameters 

`A`  

The sparse matrix, which has had values recently inserted into the object.

## Return Value

On success, SPARSE_SUCCESS, and `A` has all values inserted into the internal sparse representation.

## Discussion

Values inserted into a matrix object may not go directly into the sparse representation until needed, for example when a computation occurs. In some cases is may be beneficial to the caller to know when the cost of the update will occur. This routine allows the caller to trigger adding values to the internal sparse format.

Adding values to the sparse format can be costly, and batch updates to the matrices are recommended. Similarly, use of this routine may be expensive, so it is best to insert all values of a batch and call this routine once.

Important

Apple provides the BLAS and LAPACK libraries under the Accelerate framework to be in line with LAPACK 3.9.1. Starting with iOS 18, iPadOS 18, macOS 15, tvOS 18, watchOS 18, and visionOS 2, the libraries are in line with LAPACK 3.11.0. These new interfaces provide additional functionality, as well as a new ILP64 interface. To use the new interfaces, define `ACCELERATE_NEW_LAPACK` before including the Accelerate or vecLib headers. For ILP64 interfaces, also define `ACCELERATE_LAPACK_ILP64`. For Swift projects, specify `ACCELERATE_NEW_LAPACK=1` and `ACCELERATE_LAPACK_ILP64=1` as preprocessor macros in Xcode build settings.

## See Also

### General Sparse Matrix Management Operations

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

