

- Metal Performance Shaders
- Matrices and Vectors
-  MPSMatrixSolveLU 

Class

# MPSMatrixSolveLU

A kernel for computing the solution of a linear system of equations using an LU factorization.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSMatrixSolveLU : MPSMatrixBinaryKernel
```

## Overview

This kernel finds the solution matrix to the system *op(A) \* X = B*, where:

- *op(A)* is *Aᵀ* or *A*

- *X* is the resulting matrix of solutions

- *B* is the array of right hand sides for which the equations are to be solved

## Topics

### Initializers

init(device: any MTLDevice, transpose: Bool, order: Int, numberOfRightHandSides: Int)

### Instance Methods

func encode(commandBuffer: any MTLCommandBuffer, sourceMatrix: MPSMatrix, rightHandSideMatrix: MPSMatrix, pivotIndices: MPSMatrix, solutionMatrix: MPSMatrix)

## Relationships

### Inherits From

- MPSMatrixBinaryKernel

## See Also

### Classes for Decomposition and Solving

class MPSMatrixDecompositionCholesky

A kernel for computing the Cholesky factorization of a matrix.

class MPSMatrixSolveCholesky

A kernel for computing the solution of a linear system of equations using a Cholesky factorization.

class MPSMatrixDecompositionLU

A kernel for computing the LU factorization of a matrix using partial pivoting with row interchanges.

class MPSMatrixSolveTriangular

A kernel for computing the solution of a linear system of equations using a triangular coefficient matrix.

class MPSMatrixUnaryKernel

A kernel that consumes one matrix and produces one matrix.

class MPSMatrixBinaryKernel

A kernel that consumes two matrices and produces one matrix.

enum MPSMatrixDecompositionStatus

