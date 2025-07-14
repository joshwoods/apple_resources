

- Accelerate
- Sparse Solvers
-  Memory Management 

API Collection

# Memory Management

Retain and release sparse objects.

## Topics

### Resource Retention

func SparseRetain(SparseOpaqueSymbolicFactorization) -> SparseOpaqueSymbolicFactorization

Increases the reference count on a symbolic factorization object.

func SparseRetain(SparseOpaqueFactorization_Double) -> SparseOpaqueFactorization_Double

Increases the reference count on a double-precision numeric factorization object.

func SparseRetain(SparseOpaqueFactorization_Float) -> SparseOpaqueFactorization_Float

Increases the reference count on a single-precision numeric factorization object.

func SparseRetain(SparseOpaqueSubfactor_Double) -> SparseOpaqueSubfactor_Double

Increases the reference count on a double-precision subfactor object.

func SparseRetain(SparseOpaqueSubfactor_Float) -> SparseOpaqueSubfactor_Float

Increases the reference count on a single-precision subfactor object.

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

func SparseCleanup(SparseOpaquePreconditioner_Float)

Releases a single-precision preconditioner’s references to any memory that the Sparse Solvers library allocates.

