

- Accelerate
- Sparse Solvers
-  Transposition 

API Collection

# Transposition

Transpose matrices, factorizations, and subfactors.

## Topics

### Matrix Transpose Functions

func SparseGetTranspose(SparseMatrix_Double) -> SparseMatrix_Double

Returns a transposed copy of the specified matrix of double-precision, floating-point values.

func SparseGetTranspose(SparseMatrix_Float) -> SparseMatrix_Float

Returns a transposed copy of the specified matrix of single-precision, floating-point values.

vDSP_mtrans

Transposes a single-precision matrix.

vDSP_mtransD

Transposes a double-precision matrix.

### Factorization Transpose Functions

func SparseGetTranspose(SparseOpaqueFactorization_Double) -> SparseOpaqueFactorization_Double

Returns a transposed copy of the specified double-precision factorization.

func SparseGetTranspose(SparseOpaqueFactorization_Float) -> SparseOpaqueFactorization_Float

Returns a transposed copy of the specified single-precision factorization.

### Subfactor Transpose Functions

func SparseGetTranspose(SparseOpaqueSubfactor_Double) -> SparseOpaqueSubfactor_Double

Returns a transposed copy of the specified double-precision subfactor.

func SparseGetTranspose(SparseOpaqueSubfactor_Float) -> SparseOpaqueSubfactor_Float

Returns a transposed copy of the specified single-precision subfactor.

## See Also

### Multiplying and transposing sparse matrices

Sparse Matrix and Dense Matrix Multiplication

Multiply sparse and dense matrices.

Sparse Matrix and Dense Vector Multiplication

Multiply sparse matrices and dense vectors.

