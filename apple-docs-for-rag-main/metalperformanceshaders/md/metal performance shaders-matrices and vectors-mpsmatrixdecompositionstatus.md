

- Metal Performance Shaders
- Matrices and Vectors
-  MPSMatrixDecompositionStatus 

Enumeration

# MPSMatrixDecompositionStatus

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
enum MPSMatrixDecompositionStatus : Int32, @unchecked Sendable
```

## Topics

### Enumeration Cases

case failure

A status indicating the decomposition was not able to be completed.

case nonPositiveDefinite

A status indicating a non-positive-definite pivot value was calculated.

case singular

A status indicating the resulting decomposition is not suitable for use in a subsequent system solve.

case success

A status indicating the decomposition was performed successfully.

## Relationships

### Conforms To

- Sendable

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

class MPSMatrixUnaryKernel

A kernel that consumes one matrix and produces one matrix.

class MPSMatrixBinaryKernel

A kernel that consumes two matrices and produces one matrix.

