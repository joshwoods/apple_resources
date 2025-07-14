

- Accelerate
- Sparse Solvers
-  Subfactor Functions 

API Collection

# Subfactor Functions

Extract and work with subfactors.

## Topics

### Subfactor Extraction

struct SparseSubfactor_t

Constants that define the subfactor of a factorization.

func SparseCreateSubfactor(SparseSubfactor_t, SparseOpaqueFactorization_Double) -> SparseOpaqueSubfactor_Double

Returns an opaque object that represents a subfactor of a factorization of a matrix of double-precision values.

struct SparseOpaqueFactorization_Double

A structure that represents the factorization of a matrix of double-precision, floating-point values.

func SparseCreateSubfactor(SparseSubfactor_t, SparseOpaqueFactorization_Float) -> SparseOpaqueSubfactor_Float

Returns an opaque object that represents a subfactor of a factorization of a matrix of single-precision values.

struct SparseOpaqueFactorization_Float

A structure that represents the factorization of a matrix of single-precision, floating-point values.

### Structures

struct SparseOpaqueSubfactor_Double

struct SparseOpaqueSubfactor_Float

### Subfactor Solve and Operation Functions

Subfactor Solve Functions

Solve systems with the equation *Subfactor \* X = B*.

Subfactor Multiplication Functions

Multiply subfactors by matrices and vectors.

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

Sparse Symbolic Factorization Functions

Calculate the symbolic factorization of a matrix, and solve systems using precalculated symbolic factorizations.

Sparse Refactor Functions

Recompute a factorization using the numerical data from a matrix.

