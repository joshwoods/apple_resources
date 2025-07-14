

- Metal Performance Shaders
- Matrices and Vectors
-  MPSMatrixDecompositionLU 

Class

# MPSMatrixDecompositionLU

A kernel for computing the LU factorization of a matrix using partial pivoting with row interchanges.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSMatrixDecompositionLU : MPSMatrixUnaryKernel
```

## Overview

This kernel object computes an LU factorization, *PA = LU*, where:

- *A* is a matrix for which the LU factorization is to be computed

- *L* is a unit lower triangular matrix

- *U* is an upper triangular matrix

- *P* is a permutation matrix

## Topics

### Initializers

init(device: any MTLDevice, rows: Int, columns: Int)

### Instance Methods

func encode(commandBuffer: any MTLCommandBuffer, sourceMatrix: MPSMatrix, resultMatrix: MPSMatrix, pivotIndices: MPSMatrix, info: (any MTLBuffer)?)

## Relationships

### Inherits From

- MPSMatrixUnaryKernel

## See Also

### Classes for Decomposition and Solving

class MPSMatrixDecompositionCholesky

A kernel for computing the Cholesky factorization of a matrix.

class MPSMatrixSolveCholesky

A kernel for computing the solution of a linear system of equations using a Cholesky factorization.

class MPSMatrixSolveLU

A kernel for computing the solution of a linear system of equations using an LU factorization.

class MPSMatrixSolveTriangular

A kernel for computing the solution of a linear system of equations using a triangular coefficient matrix.

class MPSMatrixUnaryKernel

A kernel that consumes one matrix and produces one matrix.

class MPSMatrixBinaryKernel

A kernel that consumes two matrices and produces one matrix.

enum MPSMatrixDecompositionStatus

