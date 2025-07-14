

- Accelerate
- Sparse Solvers
-  Sparse Iterate Functions 

API Collection

# Sparse Iterate Functions

Perform a single iteration of the specified iterative method.

## Topics

### Sparse Iterate Functions

func SparseIterate(SparseIterativeMethod, Int32, UnsafePointer&lt;Bool>, UnsafeMutableRawPointer, (Bool, CBLAS_TRANSPOSE, DenseMatrix_Double, DenseMatrix_Double) -> Void, DenseMatrix_Double, DenseMatrix_Double, DenseMatrix_Double)

Performs a single iteration of the specified iterative method for double-precision matrices.

func SparseIterate(SparseIterativeMethod, Int32, UnsafePointer&lt;Bool>, UnsafeMutableRawPointer, (Bool, CBLAS_TRANSPOSE, DenseMatrix_Float, DenseMatrix_Float) -> Void, DenseMatrix_Float, DenseMatrix_Float, DenseMatrix_Float)

Performs a single iteration of the specified iterative method for single-precision matrices.

### Sparse Iterate Functions with Preconditioner

func SparseIterate(SparseIterativeMethod, Int32, UnsafePointer&lt;Bool>, UnsafeMutableRawPointer, (Bool, CBLAS_TRANSPOSE, DenseMatrix_Double, DenseMatrix_Double) -> Void, DenseMatrix_Double, DenseMatrix_Double, DenseMatrix_Double, SparseOpaquePreconditioner_Double)

Performs a single iteration of the specified iterative method for double-precision matrices, applying a preconditioner.

func SparseIterate(SparseIterativeMethod, Int32, UnsafePointer&lt;Bool>, UnsafeMutableRawPointer, (Bool, CBLAS_TRANSPOSE, DenseMatrix_Float, DenseMatrix_Float) -> Void, DenseMatrix_Float, DenseMatrix_Float, DenseMatrix_Float, SparseOpaquePreconditioner_Float)

Performs a single iteration of the specified iterative method for single-precision matrices, applying a preconditioner.

### Functions that Calculate Iterate State Size

func SparseGetStateSize_Double(SparseIterativeMethod, Bool, Int32, Int32, Int32) -> Int

Returns the size in bytes necessary for a call to the double-precision sparse iterate method.

func SparseGetStateSize_Float(SparseIterativeMethod, Bool, Int32, Int32, Int32) -> Int

Returns the size in bytes necessary for a call to the single-precision sparse iterate method.

## See Also

### Solving systems with iterative sparse methods

Solving systems using iterative methods

Use iterative methods to solve systems of equations where the coefficient matrix is sparse.

Sparse Iterative Solving Functions (Matrix RHS)

Solve a system with a right-hand-side dense matrix using iterative methods.

Sparse Iterative Solving Functions (Vector RHS)

Solve a system with a right-hand-side dense vector using iterative methods.

Sparse Iterative Methods

Select a suitable iterative method to solve a system.

Preconditioners

Create preconditioners for iterative solves.

