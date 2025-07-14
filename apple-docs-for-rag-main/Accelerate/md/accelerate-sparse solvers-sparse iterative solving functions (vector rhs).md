

- Accelerate
- Sparse Solvers
-  Sparse Iterative Solving Functions (Vector RHS) 

API Collection

# Sparse Iterative Solving Functions (Vector RHS)

Solve a system with a right-hand-side dense vector using iterative methods.

## Topics

### Iterative Sparse Solve Functions

func SparseSolve(SparseIterativeMethod, SparseMatrix_Double, DenseVector_Double, DenseVector_Double) -> SparseIterativeStatus_t

Solves the equation *Ax = b* for vectors of double-precision values using the specified iterative method.

func SparseSolve(SparseIterativeMethod, SparseMatrix_Float, DenseVector_Float, DenseVector_Float) -> SparseIterativeStatus_t

Solves the equation *Ax = b* for vectors of single-precision values using the specified iterative method.

func SparseSolve(SparseIterativeMethod, (Bool, CBLAS_TRANSPOSE, DenseVector_Double, DenseVector_Double) -> Void, DenseVector_Double, DenseVector_Double) -> SparseIterativeStatus_t

Solves the equation *Ax = b* for vectors of double-precision values, treating *A* as an operator and using the specified iterative method.

func SparseSolve(SparseIterativeMethod, (Bool, CBLAS_TRANSPOSE, DenseVector_Float, DenseVector_Float) -> Void, DenseVector_Float, DenseVector_Float) -> SparseIterativeStatus_t

Solves the equation *Ax = b* for vectors of single-precision values, treating *A* as an operator and using the specified iterative method.

### Iterative Sparse Solve Functions with Preconditioner

func SparseSolve(SparseIterativeMethod, SparseMatrix_Double, DenseVector_Double, DenseVector_Double, SparseOpaquePreconditioner_Double) -> SparseIterativeStatus_t

Solves the equation *Ax = b* for vectors of double-precision values using the specified iterative method and opaque preconditioner.

func SparseSolve(SparseIterativeMethod, SparseMatrix_Float, DenseVector_Float, DenseVector_Float, SparseOpaquePreconditioner_Float) -> SparseIterativeStatus_t

Solves the equation *Ax = b* for vectors of single-precision values using the specified iterative method and opaque preconditioner.

func SparseSolve(SparseIterativeMethod, SparseMatrix_Double, DenseVector_Double, DenseVector_Double, SparsePreconditioner_t) -> SparseIterativeStatus_t

Solves the equation *Ax = b* for vectors of double-precision values using the specified iterative method and preconditioner type.

func SparseSolve(SparseIterativeMethod, SparseMatrix_Float, DenseVector_Float, DenseVector_Float, SparsePreconditioner_t) -> SparseIterativeStatus_t

Solves the equation *Ax = b* for vectors of single-precision values using the specified iterative method and preconditioner type.

func SparseSolve(SparseIterativeMethod, (Bool, CBLAS_TRANSPOSE, DenseVector_Double, DenseVector_Double) -> Void, DenseVector_Double, DenseVector_Double, SparseOpaquePreconditioner_Double) -> SparseIterativeStatus_t

Solves the equation *Ax = b* for vectors of double-precision values, treating *A* as an operator and using the specified iterative method and preconditioner.

func SparseSolve(SparseIterativeMethod, (Bool, CBLAS_TRANSPOSE, DenseVector_Float, DenseVector_Float) -> Void, DenseVector_Float, DenseVector_Float, SparseOpaquePreconditioner_Float) -> SparseIterativeStatus_t

Solves the equation *Ax = b* for vectors of single-precision values, treating *A* as an operator and using the specified iterative method and preconditioner.

### Supporting Types

struct SparseIterativeStatus_t

Constants that define the status of the iterative solve.

## See Also

### Solving systems with iterative sparse methods

Solving systems using iterative methods

Use iterative methods to solve systems of equations where the coefficient matrix is sparse.

Sparse Iterative Solving Functions (Matrix RHS)

Solve a system with a right-hand-side dense matrix using iterative methods.

Sparse Iterate Functions

Perform a single iteration of the specified iterative method.

Sparse Iterative Methods

Select a suitable iterative method to solve a system.

Preconditioners

Create preconditioners for iterative solves.

