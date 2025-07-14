

- Accelerate
-  sparse_get_block_dimension_for_col(\_:\_:) 

Function

# sparse_get_block_dimension_for_col(\_:\_:)

Returns the dimension of the block for a specified column of a single-precision matrix.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func sparse_get_block_dimension_for_col(
    _ A: UnsafeMutableRawPointer!,
    _ j: sparse_index
) -> Int
```

## Parameters 

`A`  

The sparse matrix, *A*, which must have been created with sparse_matrix_block_create_float(_:_:_:_:), sparse_matrix_block_create_double(_:_:_:_:), sparse_matrix_variable_block_create_float(_:_:_:_:), or sparse_matrix_variable_block_create_double(_:_:_:_:). 0 is returned if not met. `A` holds block dimensions (fixed or variable) set with matrix object creation routine.

`j`  

The column to query.

## Return Value

The dimension of the block of the specified column.

## Discussion

Important

Apple provides the BLAS and LAPACK libraries under the Accelerate framework to be in line with LAPACK 3.9.1. Starting with iOS 18, iPadOS 18, macOS 15, tvOS 18, watchOS 18, and visionOS 2, the libraries are in line with LAPACK 3.11.0. These new interfaces provide additional functionality, as well as a new ILP64 interface. To use the new interfaces, define `ACCELERATE_NEW_LAPACK` before including the Accelerate or vecLib headers. For ILP64 interfaces, also define `ACCELERATE_LAPACK_ILP64`. For Swift projects, specify `ACCELERATE_NEW_LAPACK=1` and `ACCELERATE_LAPACK_ILP64=1` as preprocessor macros in Xcode build settings.

## See Also

### Block Dimension Queries

func sparse_get_block_dimension_for_row(UnsafeMutableRawPointer!, sparse_index) -> Int

Returns the dimension of the block for a specified row of a double-precision matrix.

