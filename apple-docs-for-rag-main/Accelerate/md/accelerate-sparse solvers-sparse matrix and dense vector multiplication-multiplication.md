

- Accelerate
- Sparse Solvers
-  Sparse Matrix and Dense Vector Multiplication 

API Collection

# Sparse Matrix and Dense Vector Multiplication

Multiply sparse matrices and dense vectors.

## Topics

### Multiplication Functions

func SparseMultiply(SparseMatrix_Double, DenseVector_Double, DenseVector_Double)

Performs the multiplication *y = Ax* on a vector of double-precision, floating-point values.

func SparseMultiply(SparseMatrix_Float, DenseVector_Float, DenseVector_Float)

Performs the multiplication *y = Ax* on a vector of single-precision, floating-point values.

func SparseMultiply(Double, SparseMatrix_Double, DenseVector_Double, DenseVector_Double)

Performs the multiply operation *y* *= alpha \* Ax* on a vector of double-precision, floating-point values.

func SparseMultiply(Float, SparseMatrix_Float, DenseVector_Float, DenseVector_Float)

Performs the multiply operation *y* *= alpha \* Ax* on a vector of single-precision, floating-point values.

### Multiply-Add Functions

func SparseMultiplyAdd(SparseMatrix_Double, DenseVector_Double, DenseVector_Double)

Performs the multiply operation *y += Ax* on a vector of double-precision, floating-point values.

func SparseMultiplyAdd(SparseMatrix_Float, DenseVector_Float, DenseVector_Float)

Performs the multiply operation *y += Ax* on a vector of double-precision, floating-point values.

func SparseMultiplyAdd(Double, SparseMatrix_Double, DenseVector_Double, DenseVector_Double)

Performs the multiply operation *y += alpha \* Ax* on a vector of double-precision, floating-point values.

func SparseMultiplyAdd(Float, SparseMatrix_Float, DenseVector_Float, DenseVector_Float)

Performs the multiply operation *y += alpha \* Ax* on a vector of single-precision, floating-point values.

## See Also

### Multiplying and transposing sparse matrices

Sparse Matrix and Dense Matrix Multiplication

Multiply sparse and dense matrices.

Transposition

Transpose matrices, factorizations, and subfactors.

