

- Metal Performance Shaders
- Matrices and Vectors
-  MPSMatrixUnaryKernel 

Class

# MPSMatrixUnaryKernel

A kernel that consumes one matrix and produces one matrix.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSMatrixUnaryKernel : MPSKernel
```

## Topics

### Instance Properties

var batchSize: Int

var batchStart: Int

var resultMatrixOrigin: MTLOrigin

var sourceMatrixOrigin: MTLOrigin

## Relationships

### Inherits From

- MPSKernel

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

class MPSMatrixSolveTriangular

A kernel for computing the solution of a linear system of equations using a triangular coefficient matrix.

class MPSMatrixBinaryKernel

A kernel that consumes two matrices and produces one matrix.

enum MPSMatrixDecompositionStatus

