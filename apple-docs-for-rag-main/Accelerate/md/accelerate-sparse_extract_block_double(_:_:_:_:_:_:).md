

- Accelerate
-  sparse_extract_block_double(\_:\_:\_:\_:\_:\_:) 

Function

# sparse_extract_block_double(\_:\_:\_:\_:\_:\_:)

Extracts values from a specified block of a double-precision matrix.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func sparse_extract_block_double(
    _ A: sparse_matrix_double!,
    _ bi: sparse_index,
    _ bj: sparse_index,
    _ row_stride: sparse_dimension,
    _ col_stride: sparse_dimension,
    _ val: UnsafeMutablePointer!
) -> sparse_status
```

## Parameters 

`A`  

The sparse matrix, *A*, which must have been created with sparse_matrix_block_create_double(_:_:_:_:) or sparse_matrix_variable_block_create_double(_:_:_:_:). SPARSE_ILLEGAL_PARAMETER is returned if not met. `A` holds block dimensions (fixed or variable) set with matrix object creation routine.

`bi`  

The block row index for value extraction. Indices are 0 based (first block of matrix is `A[0,0]`). Indices expected to be in the bounds of matrix dimensions, undefined behavior if not met.

`bj`  

The block column index for value extraction. Indices are 0 based (first block of matrix is `A[0,0]`). Indices expected to be in the bounds of matrix dimensions, undefined behavior if not met.

`row_stride`  

The row stride in number of elements to move from one row to the next for the block `val`.

`col_stride`  

The column stride in number of elements to move from one column to the next for the block `val`.

`val`  

Pointer to dense block to place the extracted values. Expected to be of size `K * L` where `K * L` is the block size for the matrix object at block index `bi,bj`. This dimensions is set at matrix object creation time.

## Return Value

On success SPARSE_SUCCESS is return and val has been updated with the block from block index `bi,bj`. If `A` creation requirements are not met, SPARSE_ILLEGAL_PARAMETER is returned and `val` is unchanged.

## Discussion

Extract the `bi,bj`’th block from the sparse matrix `A`.

Important

Apple provides the BLAS and LAPACK libraries under the Accelerate framework to be in line with LAPACK 3.9.1. Starting with iOS 18, iPadOS 18, macOS 15, tvOS 18, watchOS 18, and visionOS 2, the libraries are in line with LAPACK 3.11.0. These new interfaces provide additional functionality, as well as a new ILP64 interface. To use the new interfaces, define `ACCELERATE_NEW_LAPACK` before including the Accelerate or vecLib headers. For ILP64 interfaces, also define `ACCELERATE_LAPACK_ILP64`. For Swift projects, specify `ACCELERATE_NEW_LAPACK=1` and `ACCELERATE_LAPACK_ILP64=1` as preprocessor macros in Xcode build settings.

## See Also

### Value Extraction

func sparse_extract_block_float(sparse_matrix_float!, sparse_index, sparse_index, sparse_dimension, sparse_dimension, UnsafeMutablePointer&lt;Float>!) -> sparse_status

Extracts values from a specified block of a single-precision matrix.

