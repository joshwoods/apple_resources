

- Accelerate
- Sparse Solvers
-  Sparse Matrix and Dense Matrix Multiplication 

API Collection

# Sparse Matrix and Dense Matrix Multiplication

Multiply sparse and dense matrices.

## Topics

### Multiplication Functions

func SparseMultiply(SparseMatrix_Double, DenseMatrix_Double, DenseMatrix_Double)

Performs the multiply operation *Y* *= AX* on a sparse matrix of double-precision, floating-point values.

func SparseMultiply(SparseMatrix_Float, DenseMatrix_Float, DenseMatrix_Float)

Performs the multiply operation *Y* *= AX*\_ \_on a sparse matrix of single-precision, floating-point values.

func SparseMultiply(Double, SparseMatrix_Double, DenseMatrix_Double, DenseMatrix_Double)

Performs the multiply operation *Y = alpha \* AX* on a sparse matrix of double-precision, floating-point values.

func SparseMultiply(Float, SparseMatrix_Float, DenseMatrix_Float, DenseMatrix_Float)

Performs the multiply operation *Y = alpha \* AX* on a sparse matrix of single-precision, floating-point values.

### Multiply-Add Functions

func SparseMultiplyAdd(SparseMatrix_Double, DenseMatrix_Double, DenseMatrix_Double)

Performs the multiply operation *Y += AX* on a sparse matrix of double-precision, floating-point values.

func SparseMultiplyAdd(SparseMatrix_Float, DenseMatrix_Float, DenseMatrix_Float)

Performs the multiply operation *Y += AX* on a sparse matrix of single-precision, floating-point values.

func SparseMultiplyAdd(Double, SparseMatrix_Double, DenseMatrix_Double, DenseMatrix_Double)

Performs the multiply operation *Y += alpha \* AX* on a sparse matrix of double-precision, floating-point values.

func SparseMultiplyAdd(Float, SparseMatrix_Float, DenseMatrix_Float, DenseMatrix_Float)

Performs the multiply operation *Y += alpha \* AX* on a sparse matrix of single-precision, floating-point values.

## See Also

### Multiplying and transposing sparse matrices

Sparse Matrix and Dense Vector Multiplication

Multiply sparse matrices and dense vectors.

Transposition

Transpose matrices, factorizations, and subfactors.

