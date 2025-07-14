

- Accelerate
-  SparseConvertFromCoordinate(\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# SparseConvertFromCoordinate(\_:\_:\_:\_:\_:\_:\_:\_:)

Returns a sparse matrix of single-precision values from individual coordinate format arrays.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseConvertFromCoordinate(
    _ rowCount: Int32,
    _ columnCount: Int32,
    _ blockCount: Int,
    _ blockSize: UInt8,
    _ attributes: SparseAttributes_t,
    _ row: UnsafePointer,
    _ column: UnsafePointer,
    _ data: UnsafePointer
) -> SparseMatrix_Float
```

## Parameters 

`rowCount`  

The number of rows in the structure.

`columnCount`  

The number of columns in the structure.

`blockCount`  

The number of blocks in the matrix.

`blockSize`  

The block size for data storage on both input and output.

`attributes`  

The attributes of the matrix to create. The conversion forces the matrix to conform to the specified attributes by copying or dropping elements as necessary.

`row`  

The row indices of the matrix structure.

`column`  

The column indices of the matrix structure.

`data`  

The contents of the structurally nonzero (block) matrix elements.

## Return Value

A new SparseMatrix_Float object. After you finish using a sparse matrix, call SparseCleanup(_:) to release its references to any memory that the Sparse Solvers library allocates.

## Mentioned in 

Creating a sparse matrix from coordinate format arrays

## Discussion

The conversion drops out-of-range entries, and sums duplicate entries.

You may supply entries in either triangle for symmetric matrices. The conversion transposes entries in the triangle that triangle doesn’t specify, and sums duplicate entries.

For triangular matrices, the conversion drops entries in the triangle that triangle doesn’t specify.

## See Also

### Support for Coordinate Format Arrays

Creating a sparse matrix from coordinate format arrays

Use separate coordinate format arrays to create sparse matrices.

func SparseConvertFromCoordinate(Int32, Int32, Int, UInt8, SparseAttributes_t, UnsafePointer&lt;Int32>, UnsafePointer&lt;Int32>, UnsafePointer&lt;Double>) -> SparseMatrix_Double

Returns a sparse matrix of double-precision values from individual coordinate format arrays.

func SparseConvertFromCoordinate(Int32, Int32, Int, UInt8, SparseAttributes_t, UnsafePointer&lt;Int32>, UnsafePointer&lt;Int32>, UnsafePointer&lt;Double>, UnsafeMutableRawPointer, UnsafeMutableRawPointer) -> SparseMatrix_Double

Returns a sparse matrix of double-precision values from individual coordinate format arrays, without any internal memory allocations.

func SparseConvertFromCoordinate(Int32, Int32, Int, UInt8, SparseAttributes_t, UnsafePointer&lt;Int32>, UnsafePointer&lt;Int32>, UnsafePointer&lt;Float>, UnsafeMutableRawPointer, UnsafeMutableRawPointer) -> SparseMatrix_Float

Returns a sparse matrix of single-precision values from individual coordinate format arrays, without any internal memory allocations.

