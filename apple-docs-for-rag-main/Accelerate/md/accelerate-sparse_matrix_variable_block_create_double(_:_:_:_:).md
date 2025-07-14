

- Accelerate
-  sparse_matrix_variable_block_create_double(\_:\_:\_:\_:) 

Function

# sparse_matrix_variable_block_create_double(\_:\_:\_:\_:)

Returns a double-precision sparse matrix object that is stored in block-entry format with a variable block size.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func sparse_matrix_variable_block_create_double(
    _ Mb: sparse_dimension,
    _ Nb: sparse_dimension,
    _ K: UnsafePointer!,
    _ L: UnsafePointer!
) -> sparse_matrix_double!
```

## Parameters 

`Mb`  

The number of rows in terms of blocks of the matrix. Must be greater than 0.

`Nb`  

The number of columns in terms of blocks of the matrix. Must be greater than 0.

`K`  

Array containing row dimensions of the blocks. The `i`’th row in terms of blocks will have a dimension `K[i]`. `K` is expected to hold `Mb` elements. All values of `K` are expected to be greater than 0.

`L`  

Array containing column dimensions of the blocks. The `j`’th column in terms of blocks will have a dimension `L[j]`. `L` is expected to hold Nb elements. All values of `L` are expected to be greater than 0.

## Return Value

A matrix object that is ready for receiving entries. If an error occurs, `nil` is returned.

## Discussion

Create a sparse matrix object that is stored in block-entry format and is ready to receive values from the various block insert routines. Blocks are are of variable dimension where the `i,j`’th block index has a dimension `K[i] * L[j]`. Block-entry format means blocks of dense regions will be stored at block indices `i,j`. For point wise format use non block version of create. See the various insert routines for details on inserting values into this matrix object.

Important

Apple provides the BLAS and LAPACK libraries under the Accelerate framework to be in line with LAPACK 3.9.1. Starting with iOS 18, iPadOS 18, macOS 15, tvOS 18, watchOS 18, and visionOS 2, the libraries are in line with LAPACK 3.11.0. These new interfaces provide additional functionality, as well as a new ILP64 interface. To use the new interfaces, define `ACCELERATE_NEW_LAPACK` before including the Accelerate or vecLib headers. For ILP64 interfaces, also define `ACCELERATE_LAPACK_ILP64`. For Swift projects, specify `ACCELERATE_NEW_LAPACK=1` and `ACCELERATE_LAPACK_ILP64=1` as preprocessor macros in Xcode build settings.

## See Also

### Matrix Creation and Population

func sparse_matrix_block_create_double(sparse_dimension, sparse_dimension, sparse_dimension, sparse_dimension) -> sparse_matrix_double!

Returns a double-precision sparse matrix object that is stored in block-entry format with a fixed block size.

func sparse_matrix_block_create_float(sparse_dimension, sparse_dimension, sparse_dimension, sparse_dimension) -> sparse_matrix_float!

Returns a single-precision sparse matrix object that is stored in block-entry format with a fixed block size.

func sparse_matrix_variable_block_create_float(sparse_dimension, sparse_dimension, UnsafePointer&lt;sparse_dimension>!, UnsafePointer&lt;sparse_dimension>!) -> sparse_matrix_float!

Returns a single-precision sparse matrix object that is stored in block-entry format with a variable block size.

func sparse_insert_block_double(sparse_matrix_double!, UnsafePointer&lt;Double>!, sparse_dimension, sparse_dimension, sparse_index, sparse_index) -> sparse_status

Inserts a dense block of entries into a double-precision matrix.

func sparse_insert_block_float(sparse_matrix_float!, UnsafePointer&lt;Float>!, sparse_dimension, sparse_dimension, sparse_index, sparse_index) -> sparse_status

Inserts a dense block of entries into a single-precision matrix.

