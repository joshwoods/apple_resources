

- Metal Performance Shaders
- Matrices and Vectors
-  MPSMatrixDecompositionCholesky 

Class

# MPSMatrixDecompositionCholesky

A kernel for computing the Cholesky factorization of a matrix.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSMatrixDecompositionCholesky : MPSMatrixUnaryKernel
```

## Overview

This kernel computes one of the following factorizations of a matrix *A*:

- *A = LLᵀ*

- *A = UᵀU*

where:

- *A* is a symmetric positive-definite matrix for which the factorization is to be computed

- *L* is the lower triangular matrix

- *U* is the upper triangular matrix

## Topics

### Initializers

init(device: any MTLDevice, lower: Bool, order: Int)

### Instance Methods

func encode(commandBuffer: any MTLCommandBuffer, sourceMatrix: MPSMatrix, resultMatrix: MPSMatrix, status: (any MTLBuffer)?)

## Relationships

### Inherits From

- MPSMatrixUnaryKernel

## See Also

### Classes for Decomposition and Solving

class MPSMatrixSolveCholesky

A kernel for computing the solution of a linear system of equations using a Cholesky factorization.

class MPSMatrixDecompositionLU

A kernel for computing the LU factorization of a matrix using partial pivoting with row interchanges.

class MPSMatrixSolveLU

A kernel for computing the solution of a linear system of equations using an LU factorization.

class MPSMatrixSolveTriangular

A kernel for computing the solution of a linear system of equations using a triangular coefficient matrix.

class MPSMatrixUnaryKernel

A kernel that consumes one matrix and produces one matrix.

class MPSMatrixBinaryKernel

A kernel that consumes two matrices and produces one matrix.

enum MPSMatrixDecompositionStatus

