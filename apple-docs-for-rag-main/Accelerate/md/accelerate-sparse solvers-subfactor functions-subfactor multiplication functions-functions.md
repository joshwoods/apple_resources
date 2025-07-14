

- Accelerate
- Sparse Solvers
- Subfactor Functions
-  Subfactor Multiplication Functions 

API Collection

# Subfactor Multiplication Functions

Multiply subfactors by matrices and vectors.

## Topics

### Subfactor and Dense Matrix Multiplication

func SparseMultiply(SparseOpaqueSubfactor_Double, DenseMatrix_Double)

Performs the multiply operation *Y* *= Subfactor \* X,* \_\_in place on a dense matrix of double-precision values.

func SparseMultiply(SparseOpaqueSubfactor_Float, DenseMatrix_Float)

Performs the multiply operation *Y*\_ \_*= Subfactor \* X*, in place on a dense matrix of single-precision values.

func SparseMultiply(SparseOpaqueSubfactor_Double, DenseMatrix_Double, DenseMatrix_Double)

Performs the multiply operation *Y* *= Subfactor \* X* on a dense matrix of double-precision values.

func SparseMultiply(SparseOpaqueSubfactor_Float, DenseMatrix_Float, DenseMatrix_Float)

Performs the multiply operation *Y* *= Subfactor \* X* on a dense matrix of single-precision values.

### Subfactor and Dense Matrix Multiplication with User-Defined Workspace

func SparseMultiply(SparseOpaqueSubfactor_Double, DenseMatrix_Double, UnsafeMutableRawPointer)

Performs the multiply operation *Y* *= Subfactor \* X*, in place on a dense matrix of double-precision values and without any internal memory allocations.

func SparseMultiply(SparseOpaqueSubfactor_Float, DenseMatrix_Float, UnsafeMutableRawPointer)

Performs the multiply operation *Y* *= Subfactor \* X*, in place on a dense matrix of single-precision values and without any internal memory allocations.

func SparseMultiply(SparseOpaqueSubfactor_Double, DenseMatrix_Double, DenseMatrix_Double, UnsafeMutableRawPointer)

Performs the multiply operation *Y* *= Subfactor \* X* on a dense matrix of double-precision values and without any internal memory allocations.

func SparseMultiply(SparseOpaqueSubfactor_Float, DenseMatrix_Float, DenseMatrix_Float, UnsafeMutableRawPointer)

Performs the multiply operation *Y* *= Subfactor \* X* on a dense matrix of single-precision values and without any internal memory allocations.

### Subfactor and Dense Vector Multiplication

func SparseMultiply(SparseOpaqueSubfactor_Double, DenseVector_Double)

Performs the multiply operation *Y = Subfactor \* X*, in place on a vector of double-precision values.

func SparseMultiply(SparseOpaqueSubfactor_Float, DenseVector_Float)

Performs the multiply operation *Y = Subfactor \* X*, in place on a vector of single-precision values.

func SparseMultiply(SparseOpaqueSubfactor_Double, DenseVector_Double, DenseVector_Double)

Performs the multiply operation *Y = Subfactor \* X* on a vector of double-precision values.

func SparseMultiply(SparseOpaqueSubfactor_Float, DenseVector_Float, DenseVector_Float)

Performs the multiply operation *Y = Subfactor \** *X* on a vector of single-precision values.

### Subfactor and Dense Vector Multiplication with User-Defined Workspace

func SparseMultiply(SparseOpaqueSubfactor_Double, DenseVector_Double, UnsafeMutableRawPointer)

Performs the multiply operation *Y = Subfactor \* X* on a vector of double-precision values *X*, in place and without any internal memory allocations.

func SparseMultiply(SparseOpaqueSubfactor_Float, DenseVector_Float, UnsafeMutableRawPointer)

Performs the multiply operation *Y = Subfactor \* X* on a vector of single-precision values *X*, in place and without any internal memory allocations.

func SparseMultiply(SparseOpaqueSubfactor_Double, DenseVector_Double, DenseVector_Double, UnsafeMutableRawPointer)

Performs the multiply operation *Y = Subfactor \* X* on a vector of double-precision values *X*, without any internal memory allocations.

func SparseMultiply(SparseOpaqueSubfactor_Float, DenseVector_Float, DenseVector_Float, UnsafeMutableRawPointer)

Performs the multiply operation *Y = Subfactor \* X* on a vector of double-precision values *X*, without any internal memory allocations.

## See Also

### Subfactor Solve and Operation Functions

Subfactor Solve Functions

Solve systems with the equation *Subfactor \* X = B*.

