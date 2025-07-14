

- Accelerate
-  sparse_insert_block_float(\_:\_:\_:\_:\_:\_:) 

Function

# sparse_insert_block_float(\_:\_:\_:\_:\_:\_:)

Inserts a dense block of entries into a single-precision matrix.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func sparse_insert_block_float(
    _ A: sparse_matrix_float!,
    _ val: UnsafePointer!,
    _ row_stride: sparse_dimension,
    _ col_stride: sparse_dimension,
    _ bi: sparse_index,
    _ bj: sparse_index
) -> sparse_status
```

## Parameters 

`A`  

The sparse matrix, *A*,\_ \_which must have been created with sparse_matrix_block_create_float(_:_:_:_:) or sparse_matrix_variable_block_create_float(_:_:_:_:). SPARSE_ILLEGAL_PARAMETER is returned if not met. `A` holds block dimensions (fixed or variable) set with matrix object creation routine.

`val`  

Pointer to block to be inserted at block index location `A[bi,bj]`. The block is of dimension `k * l` where `k` and `l` are set for `bi,bj` at object creation time. The strides between elements for rows and columns are provided in `row_stride` and `col_stride`.

`row_stride`  

The row stride in number of elements to move from one row to the next for the block `val`.

`col_stride`  

The column stride in number of elements to move from one column to the next for the block `val`.

`bi`  

The block row index where `val` is to be inserted. Indexing is zero based, the first block is located at `0,0`. Index is assumed to be within the bounds of the matrix object, undefined behavior if not met.

`bj`  

The block column index where `val` is to be inserted. Indexing is zero based, the first block is located at `0,0`. Index is assumed to be within the bounds of the matrix object, undefined behavior if not met.

## Return Value

On successful insertion, `A` has been updated with the value and SPARSE_SUCCESS is returned. If `A` creation requirements are not met, SPARSE_ILLEGAL_PARAMETER is returned and `A` is unchanged.

## Discussion

Use to build a sparse matrix by providing a dense block for entry at block location `A[bi,bj]`. Block size is determined at object creation time. Given a block dimension of `k * l` and for location `bi,bj`, update as: `A[bi,bj][i,j] = val[i*row_stride + j*col_stride]` for each `i` in `k` and each `j` in `l`.

Note that matrix properties cannot be modified after value insertion begins.This includes properties such as specifying a triangular matrix.Insertion can be expensive, generally speaking it is best to do a batch update. Inserted values may be temporarily held internally within the object and only inserted into the sparse format when a later computation triggers a need to insert.

Important

Apple provides the BLAS and LAPACK libraries under the Accelerate framework to be in line with LAPACK 3.9.1. Starting with iOS 18, iPadOS 18, macOS 15, tvOS 18, watchOS 18, and visionOS 2, the libraries are in line with LAPACK 3.11.0. These new interfaces provide additional functionality, as well as a new ILP64 interface. To use the new interfaces, define `ACCELERATE_NEW_LAPACK` before including the Accelerate or vecLib headers. For ILP64 interfaces, also define `ACCELERATE_LAPACK_ILP64`. For Swift projects, specify `ACCELERATE_NEW_LAPACK=1` and `ACCELERATE_LAPACK_ILP64=1` as preprocessor macros in Xcode build settings.

## See Also

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

