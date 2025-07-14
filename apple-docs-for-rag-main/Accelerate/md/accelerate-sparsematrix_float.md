

- Accelerate
-  SparseMatrix_Float 

Structure

# SparseMatrix_Float

A structure that contains a sparse matrix of single-precision, floating-point values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseMatrix_Float
```

## Overview

You typically use sparse matrices to represent the sparse coefficient matrix in the matrix equation *Ax = b.* A SparseMatrix_Float structure provides a pointer to its underlying data, and information about its structure and attributes.

The Accelerate framework uses the compressed sparse column (CSC) format to store sparse matrices. CSC stores the matrix as a series of column vectors that specifies only the nonzero entries as `(row-index, value)` pairs. For more information, see Creating sparse matrices.

After you finish using a sparse matrix, call SparseCleanup(_:) to release its references to any memory that the Sparse Solvers library allocates.

## Topics

### Creating a Sparse Matrix

init(structure: SparseMatrixStructure, data: UnsafeMutablePointer&lt;Float>)

Creates a sparse matrix with the specified structure that contains single-precision values.

### Inspecting a Matrix’s Structure and Data

var structure: SparseMatrixStructure

The sparsity structure of the matrix.

var data: UnsafeMutablePointer&lt;Float>

The array of contiguous values in the nonzero blocks of the matrix.

### Specifying the Structure and Attributes of a Sparse Matrix

struct SparseMatrixStructure

A description of the sparsity structure of a sparse matrix.

struct SparseAttributes_t

A structure that represents the attributes of a matrix.

## See Also

### Creating sparse matrices

Creating sparse matrices

Create sparse matrices for factorization and solving systems.

struct SparseMatrix_Double

A structure that contains a sparse matrix of double-precision, floating-point values.

Conversion from Other Formats

Create sparse matrices from coordinate format arrays and BLAS opaque matrices.

