

- Accelerate
-  SparseCleanup(\_:) 

Function

# SparseCleanup(\_:)

Releases a single-precision preconditioner’s references to any memory that the Sparse Solvers library allocates.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseCleanup(_ Preconditioner: SparseOpaquePreconditioner_Float)
```

## Parameters 

`Preconditioner`  

The preconditioner to release references to any allocated memory.

## See Also

### Resource Cleanup

func SparseCleanup(SparseMatrix_Double)

Releases a matrix of double-precision values’ references to any memory that the Sparse Solvers library allocates.

func SparseCleanup(SparseMatrix_Float)

Releases a matrix of single-precision values’ references to any memory that the Sparse Solvers library allocates.

func SparseCleanup(SparseOpaqueFactorization_Double)

Releases a factorization of a matrix of double-precision values’ references to any memory that the Sparse Solvers library allocates.

func SparseCleanup(SparseOpaqueFactorization_Float)

Releases a factorization of a matrix of single-precision values’ references to any memory that the Sparse Solvers library allocates.

func SparseCleanup(SparseOpaqueSymbolicFactorization)

Releases a matrix factorization’s references to any memory that the Sparse Solvers library allocates.

func SparseCleanup(SparseOpaqueSubfactor_Double)

Releases a double-precision subfactor object’s references to any memory that the Sparse Solvers library allocates.

func SparseCleanup(SparseOpaqueSubfactor_Float)

Releases a single-precision subfactor object’s references to any memory that the Sparse Solvers library allocates.

func SparseCleanup(SparseOpaquePreconditioner_Double)

Releases a double-precision preconditioner’s references to any memory that the Sparse Solvers library allocates.

