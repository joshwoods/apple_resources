

- Accelerate
-  SparseMatrixStructure 

Structure

# SparseMatrixStructure

A description of the sparsity structure of a sparse matrix.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseMatrixStructure
```

## Mentioned in 

Creating sparse matrices

## Overview

The sparsity structure is in a *block compressed sparse column* format. The matrix consists of rowCount x columnCount blocks, each of which is a square matrix of some fixed size. The system stores this block size separately from the sparsity because the graph algorithms that operate on the structure don’t need it.

## Topics

### Creating a sparse matrix description

init(rowCount: Int32, columnCount: Int32, columnStarts: UnsafeMutablePointer&lt;Int>, rowIndices: UnsafeMutablePointer&lt;Int32>, attributes: SparseAttributes_t, blockSize: UInt8)

Creates a new structure that represents the sparsity structure of a sparse matrix.

### Inspecting the properties of a sparse matrix description

var attributes: SparseAttributes_t

The attributes of the matrix, such as whether it’s symmetrical or triangular.

var blockSize: UInt8

The block size of the matrix.

var columnCount: Int32

The number of columns in the matrix.

var columnStarts: UnsafeMutablePointer&lt;Int>

The starting index for each column in the row indices array.

var rowCount: Int32

The number of rows in the matrix.

var rowIndices: UnsafeMutablePointer&lt;Int32>

The row indices of the matrix.

## See Also

### Related Documentation

Creating sparse matrices

Create sparse matrices for factorization and solving systems.

### Specifying the Structure and Attributes of a Sparse Matrix

struct SparseAttributes_t

A structure that represents the attributes of a matrix.

