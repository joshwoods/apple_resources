

- Accelerate
- Sparse Solvers
-  Sparse Symbolic Factorization Functions 

API Collection

# Sparse Symbolic Factorization Functions

Calculate the symbolic factorization of a matrix, and solve systems using precalculated symbolic factorizations.

## Topics

### Matrix Symbolic Factorization Functions

func SparseFactor(SparseFactorization_t, SparseMatrixStructure) -> SparseOpaqueSymbolicFactorization

Returns a symbolic factorization of the requested type for a specified sparsity structure.

func SparseFactor(SparseFactorization_t, SparseMatrixStructure, SparseSymbolicFactorOptions) -> SparseOpaqueSymbolicFactorization

Returns a symbolic factorization of the requested type for a single-precision matrix with the specified structure.

### Matrix Factorizations Using Precalculated Symbolic Factorization

func SparseFactor(SparseOpaqueSymbolicFactorization, SparseMatrix_Double) -> SparseOpaqueFactorization_Double

Returns the factorization of a sparse matrix of double-precision values that corresponds to the supplied symbolic factorization.

func SparseFactor(SparseOpaqueSymbolicFactorization, SparseMatrix_Float) -> SparseOpaqueFactorization_Float

Returns the factorization of a sparse matrix of single-precision values that corresponds to the supplied symbolic factorization.

func SparseFactor(SparseOpaqueSymbolicFactorization, SparseMatrix_Double, SparseNumericFactorOptions) -> SparseOpaqueFactorization_Double

Returns the factorization of a sparse matrix of double-precision values that corresponds to the supplied symbolic factorization using specified options.

func SparseFactor(SparseOpaqueSymbolicFactorization, SparseMatrix_Float, SparseNumericFactorOptions) -> SparseOpaqueFactorization_Float

Returns the factorization of a sparse matrix of single-precision values that corresponds to the supplied symbolic factorization using specified options.

### Matrix Factorizations Using Precalculated Symbolic Factorization with User-Defined Workspace

func SparseFactor(SparseOpaqueSymbolicFactorization, SparseMatrix_Double, SparseNumericFactorOptions, UnsafeMutableRawPointer?, UnsafeMutableRawPointer?) -> SparseOpaqueFactorization_Double

Returns the factorization of a sparse matrix of double-precision values that corresponds to the supplied symbolic factorization using user-defined workspace and factor storage.

func SparseFactor(SparseOpaqueSymbolicFactorization, SparseMatrix_Float, SparseNumericFactorOptions, UnsafeMutableRawPointer?, UnsafeMutableRawPointer?) -> SparseOpaqueFactorization_Float

Returns the factorization of a sparse matrix of single-precision values that corresponds to the supplied symbolic factorization using user-defined workspace and factor storage.

### Supporting Types

struct SparseOpaqueSymbolicFactorization

A semi-opaque type that represents symbolic matrix factorization.

struct SparseFactorization_t

Constants that define the factorization type.

struct SparseSymbolicFactorOptions

A structure that contains options that affect the symbolic stage of a sparse factorization.

## See Also

### Solving systems with direct sparse methods

Solving systems using direct methods

Use direct methods to solve systems of equations where the coefficient matrix is sparse.

struct SparseOpaqueFactorization_Double

A structure that represents the factorization of a matrix of double-precision, floating-point values.

struct SparseOpaqueFactorization_Float

A structure that represents the factorization of a matrix of single-precision, floating-point values.

Sparse Matrix Factor Functions

Compute the factorization of a matrix.

Sparse Direct Solving Functions (Matrix RHS)

Solve a system with a right-hand-side dense matrix using a factored sparse coefficient matrix.

Sparse Direct Solving Functions (Vector RHS)

Solve a system with a right-hand-side dense vector using a factored sparse coefficient matrix.

Sparse Refactor Functions

Recompute a factorization using the numerical data from a matrix.

Subfactor Functions

Extract and work with subfactors.

