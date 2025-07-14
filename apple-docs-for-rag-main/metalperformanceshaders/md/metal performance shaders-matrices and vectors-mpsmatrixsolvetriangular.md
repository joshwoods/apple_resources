

- Metal Performance Shaders
- Matrices and Vectors
-  MPSMatrixSolveTriangular 

Class

# MPSMatrixSolveTriangular

A kernel for computing the solution of a linear system of equations using a triangular coefficient matrix.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSMatrixSolveTriangular : MPSMatrixBinaryKernel
```

## Overview

This kernel finds the solution matrix to the system *op(A) \* X = alpha \* B* or *X \* op(A) = alpha \* B*, where:

- A is either an upper or lower triangular matrix

- *op(A)* is either *Aᵀ* or *A*

- *X* is the resulting matrix of solutions

- *B* is the array of right hand sides for which the equations are to be solved

## Topics

### Initializers

init(device: any MTLDevice, right: Bool, upper: Bool, transpose: Bool, unit: Bool, order: Int, numberOfRightHandSides: Int, alpha: Double)

### Instance Methods

func encode(commandBuffer: any MTLCommandBuffer, sourceMatrix: MPSMatrix, rightHandSideMatrix: MPSMatrix, solutionMatrix: MPSMatrix)

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

class MPSMatrixSolveLU

A kernel for computing the solution of a linear system of equations using an LU factorization.

class MPSMatrixUnaryKernel

A kernel that consumes one matrix and produces one matrix.

class MPSMatrixBinaryKernel

A kernel that consumes two matrices and produces one matrix.

enum MPSMatrixDecompositionStatus

