

- Accelerate
- Sparse Solvers
-  Sparse Refactor Functions 

API Collection

# Sparse Refactor Functions

Recompute a factorization using the numerical data from a matrix.

## Topics

### Matrix Refactorization Functions

func SparseRefactor(SparseMatrix_Double, UnsafeMutablePointer&lt;SparseOpaqueFactorization_Double>)

Computes a factorization of the specified double-precision matrix using an existing factorization’s storage.

func SparseRefactor(SparseMatrix_Float, UnsafeMutablePointer&lt;SparseOpaqueFactorization_Float>)

Computes a factorization of the specified single-precision matrix using an existing factorization’s storage.

func SparseRefactor(SparseMatrix_Double, UnsafeMutablePointer&lt;SparseOpaqueFactorization_Double>, SparseNumericFactorOptions)

Computes a factorization of the specified double-precision matrix using an existing factorization’s storage and specified options.

func SparseRefactor(SparseMatrix_Float, UnsafeMutablePointer&lt;SparseOpaqueFactorization_Float>, SparseNumericFactorOptions)

Computes a factorization of the specified single-precision matrix using an existing factorization’s storage and specified options.

### Matrix Refactorizations Functions with User-Defined Workspace

func SparseRefactor(SparseMatrix_Double, UnsafeMutablePointer&lt;SparseOpaqueFactorization_Double>, UnsafeMutableRawPointer)

Computes a factorization of the specified double-precision matrix using an existing factorization’s storage, without internal memory allocation.

func SparseRefactor(SparseMatrix_Float, UnsafeMutablePointer&lt;SparseOpaqueFactorization_Float>, UnsafeMutableRawPointer)

Computes a factorization of the specified single-precision matrix using an existing factorization’s storage, without internal memory allocation.

func SparseRefactor(SparseMatrix_Double, UnsafeMutablePointer&lt;SparseOpaqueFactorization_Double>, SparseNumericFactorOptions, UnsafeMutableRawPointer)

Computes a factorization of the specified double-precision matrix using an existing factorization’s storage and specified options, and without internal memory allocation.

func SparseRefactor(SparseMatrix_Float, UnsafeMutablePointer&lt;SparseOpaqueFactorization_Float>, SparseNumericFactorOptions, UnsafeMutableRawPointer)

Computes a factorization of the specified single-precision matrix using an existing factorization’s storage and specified options, and without internal memory allocation.

### Numeric Factorization Options

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

Sparse Matrix Factor Functions

Compute the factorization of a matrix.

Sparse Direct Solving Functions (Matrix RHS)

Solve a system with a right-hand-side dense matrix using a factored sparse coefficient matrix.

Sparse Direct Solving Functions (Vector RHS)

Solve a system with a right-hand-side dense vector using a factored sparse coefficient matrix.

Sparse Symbolic Factorization Functions

Calculate the symbolic factorization of a matrix, and solve systems using precalculated symbolic factorizations.

Subfactor Functions

Extract and work with subfactors.

