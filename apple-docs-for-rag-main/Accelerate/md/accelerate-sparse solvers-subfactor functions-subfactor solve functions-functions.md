

- Accelerate
- Sparse Solvers
- Subfactor Functions
-  Subfactor Solve Functions 

API Collection

# Subfactor Solve Functions

Solve systems with the equation *Subfactor \* X = B*.

## Topics

### Matrix Solve Functions

func SparseSolve(SparseOpaqueSubfactor_Double, DenseMatrix_Double)

Solves the equation *Subfactor \* X = B* in place for the matrix of double-precision values *X*.

func SparseSolve(SparseOpaqueSubfactor_Float, DenseMatrix_Float)

Solves the equation *Subfactor \* X = B* in place for the matrix of single-precision values *X*.

func SparseSolve(SparseOpaqueSubfactor_Double, DenseMatrix_Double, DenseMatrix_Double)

Solves the equation *Subfactor \* X = B* for the matrix of double-precision values *X*.

func SparseSolve(SparseOpaqueSubfactor_Float, DenseMatrix_Float, DenseMatrix_Float)

Solves the equation *Subfactor \* X = B* for the matrix of single-precision values *X*.

### Matrix Solve Functions with User-Defined Workspace

func SparseSolve(SparseOpaqueSubfactor_Double, DenseMatrix_Double, UnsafeMutableRawPointer)

Solves the equation *Subfactor \* X = B* in place for the matrix of double-precision values *X*, without any internal memory allocations.

func SparseSolve(SparseOpaqueSubfactor_Float, DenseMatrix_Float, UnsafeMutableRawPointer)

Solves the equation *Subfactor \* X = B* in place for the matrix of single-precision values *X*, without any internal memory allocations.

func SparseSolve(SparseOpaqueSubfactor_Double, DenseMatrix_Double, DenseMatrix_Double, UnsafeMutableRawPointer)

Solves the equation *Subfactor \* X = B* for the matrix of double-precision values *X*, without any internal memory allocations.

func SparseSolve(SparseOpaqueSubfactor_Float, DenseMatrix_Float, DenseMatrix_Float, UnsafeMutableRawPointer)

Solves the equation *Subfactor \* X = B* for the matrix of single-precision values *X*, without any internal memory allocations.

### Vector Solve Functions

func SparseSolve(SparseOpaqueSubfactor_Double, DenseVector_Double)

Solves the equation *Subfactor \* X = B* in place for the vector of double-precision values *X*.

func SparseSolve(SparseOpaqueSubfactor_Float, DenseVector_Float)

Solves the equation *Subfactor \* X = B* in place for the vector of single-precision values *X*.

func SparseSolve(SparseOpaqueSubfactor_Double, DenseVector_Double, DenseVector_Double)

Solves the equation *Subfactor \* X = B* in place for the vector of double-precision values *X*.

func SparseSolve(SparseOpaqueSubfactor_Float, DenseVector_Float, DenseVector_Float)

Solves the equation *Subfactor \* X = B* in place for the vector of single-precision values *X*.

### Vector Solve Functions with User-Defined Workspace

func SparseSolve(SparseOpaqueSubfactor_Double, DenseVector_Double, UnsafeMutableRawPointer)

Solves the equation *Subfactor \* X = B* for the vector of double-precision values *X*, in place and without any internal memory allocations.

func SparseSolve(SparseOpaqueSubfactor_Float, DenseVector_Float, UnsafeMutableRawPointer)

Solves the equation *Subfactor \* X = B* for the vector of single-precision values *X*, in place and without any internal memory allocations.

func SparseSolve(SparseOpaqueSubfactor_Double, DenseVector_Double, DenseVector_Double, UnsafeMutableRawPointer)

Solves the equation *Subfactor \* X = B* for the vector of double-precision values *X*, without any internal memory allocations.

func SparseSolve(SparseOpaqueSubfactor_Float, DenseVector_Float, DenseVector_Float, UnsafeMutableRawPointer)

Solves the equation *Subfactor \* X = B* for the vector of single-precision values *X*, without any internal memory allocations.

## See Also

### Subfactor Solve and Operation Functions

Subfactor Multiplication Functions

Multiply subfactors by matrices and vectors.

