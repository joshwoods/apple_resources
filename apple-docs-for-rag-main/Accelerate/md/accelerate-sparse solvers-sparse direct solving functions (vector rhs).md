

- Accelerate
- Sparse Solvers
-  Sparse Direct Solving Functions (Vector RHS) 

API Collection

# Sparse Direct Solving Functions (Vector RHS)

Solve a system with a right-hand-side dense vector using a factored sparse coefficient matrix.

## Topics

### In-Place Direct Solving Functions

func SparseSolve(SparseOpaqueFactorization_Double, DenseVector_Double)

Solves the system *Ax = x* using the supplied double-precision factorization of *A*.

func SparseSolve(SparseOpaqueFactorization_Float, DenseVector_Float)

Solves the system *Ax = b* using the supplied single-precision factorization of *A*, in place.

### Out-of-Place Direct Solving Functions

func SparseSolve(SparseOpaqueFactorization_Double, DenseVector_Double, DenseVector_Double)

Solves the system *Ax = b* using the supplied double-precision factorization of *A*.

func SparseSolve(SparseOpaqueFactorization_Float, DenseVector_Float, DenseVector_Float)

Solves the system *Ax = b* using the supplied single-precision factorization of *A*.

### In-Place Direct Solving Functions with User-Defined Workspace

func SparseSolve(SparseOpaqueFactorization_Double, DenseVector_Double, UnsafeMutableRawPointer)

Solves the system *Ax = b* using the supplied double-precision factorization of *A*, in place and without any internal memory allocations.

func SparseSolve(SparseOpaqueFactorization_Float, DenseVector_Float, UnsafeMutableRawPointer)

Solves the system *Ax = b* using the supplied single-precision factorization of *A*, in place and without any internal memory allocations.

### Out-of-Place Direct Solving Functions with User-Defined Workspace

func SparseSolve(SparseOpaqueFactorization_Double, DenseVector_Double, DenseVector_Double, UnsafeMutableRawPointer)

Solves the system *Ax = b* using the supplied double-precision factorization of *A*, without any internal memory allocations.

func SparseSolve(SparseOpaqueFactorization_Float, DenseVector_Float, DenseVector_Float, UnsafeMutableRawPointer)

Solves the system *Ax = b* using the supplied single-precision factorization of *A*, without any internal memory allocations.

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

Sparse Symbolic Factorization Functions

Calculate the symbolic factorization of a matrix, and solve systems using precalculated symbolic factorizations.

Sparse Refactor Functions

Recompute a factorization using the numerical data from a matrix.

Subfactor Functions

Extract and work with subfactors.

