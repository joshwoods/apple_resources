

- Accelerate
- Sparse Solvers
-  Sparse Matrix Factor Functions 

API Collection

# Sparse Matrix Factor Functions

Compute the factorization of a matrix.

## Topics

### Matrix Factorization Functions

func SparseFactor(SparseFactorization_t, SparseMatrix_Double) -> SparseOpaqueFactorization_Double

Returns the specified factorization of a sparse matrix of double-precision values.

func SparseFactor(SparseFactorization_t, SparseMatrix_Float) -> SparseOpaqueFactorization_Float

Returns the specified factorization of a sparse matrix of single-precision values.

func SparseFactor(SparseFactorization_t, SparseMatrix_Double, SparseSymbolicFactorOptions, SparseNumericFactorOptions) -> SparseOpaqueFactorization_Double

Returns the specified factorization of a sparse matrix of double-precision values using the specified options.

func SparseFactor(SparseFactorization_t, SparseMatrix_Float, SparseSymbolicFactorOptions, SparseNumericFactorOptions) -> SparseOpaqueFactorization_Float

Returns the specified factorization of a sparse matrix of single-precision values using the specified options.

### Factorization Intertia Functions

func SparseGetInertia(SparseOpaqueFactorization_Float, UnsafeMutablePointer&lt;Int32>, UnsafeMutablePointer&lt;Int32>, UnsafeMutablePointer&lt;Int32>) -> Int32

Returns the inertia of a single-precision *LDLᵀ* factorization.

func SparseGetInertia(SparseOpaqueFactorization_Double, UnsafeMutablePointer&lt;Int32>, UnsafeMutablePointer&lt;Int32>, UnsafeMutablePointer&lt;Int32>) -> Int32

Returns the inertia of a double-precision *LDLᵀ* factorization.

### Structures that Specify Factorization Type and Factorization Options

struct SparseFactorization_t

Constants that define the factorization type.

struct SparseSymbolicFactorOptions

A structure that contains options that affect the symbolic stage of a sparse factorization.

struct SparseNumericFactorOptions

A structure that contains options that affect the numerical stage of a sparse factorization.

## See Also

### Solving systems with direct sparse methods

Solving systems using direct methods

Use direct methods to solve systems of equations where the coefficient matrix is sparse.

struct SparseOpaqueFactorization_Double

A structure that represents the factorization of a matrix of double-precision, floating-point values.

struct SparseOpaqueFactorization_Float

A structure that represents the factorization of a matrix of single-precision, floating-point values.

Sparse Direct Solving Functions (Matrix RHS)

Solve a system with a right-hand-side dense matrix using a factored sparse coefficient matrix.

Sparse Direct Solving Functions (Vector RHS)

Solve a system with a right-hand-side dense vector using a factored sparse coefficient matrix.

Sparse Symbolic Factorization Functions

Calculate the symbolic factorization of a matrix, and solve systems using precalculated symbolic factorizations.

Sparse Refactor Functions

Recompute a factorization using the numerical data from a matrix.

Subfactor Functions

Extract and work with subfactors.

