

- Accelerate
- Sparse Solvers
-  Conversion from Other Formats 

API Collection

# Conversion from Other Formats

Create sparse matrices from coordinate format arrays and BLAS opaque matrices.

## Topics

### Support for Coordinate Format Arrays

Creating a sparse matrix from coordinate format arrays

Use separate coordinate format arrays to create sparse matrices.

func SparseConvertFromCoordinate(Int32, Int32, Int, UInt8, SparseAttributes_t, UnsafePointer&lt;Int32>, UnsafePointer&lt;Int32>, UnsafePointer&lt;Double>) -> SparseMatrix_Double

Returns a sparse matrix of double-precision values from individual coordinate format arrays.

func SparseConvertFromCoordinate(Int32, Int32, Int, UInt8, SparseAttributes_t, UnsafePointer&lt;Int32>, UnsafePointer&lt;Int32>, UnsafePointer&lt;Float>) -> SparseMatrix_Float

Returns a sparse matrix of single-precision values from individual coordinate format arrays.

func SparseConvertFromCoordinate(Int32, Int32, Int, UInt8, SparseAttributes_t, UnsafePointer&lt;Int32>, UnsafePointer&lt;Int32>, UnsafePointer&lt;Double>, UnsafeMutableRawPointer, UnsafeMutableRawPointer) -> SparseMatrix_Double

Returns a sparse matrix of double-precision values from individual coordinate format arrays, without any internal memory allocations.

func SparseConvertFromCoordinate(Int32, Int32, Int, UInt8, SparseAttributes_t, UnsafePointer&lt;Int32>, UnsafePointer&lt;Int32>, UnsafePointer&lt;Float>, UnsafeMutableRawPointer, UnsafeMutableRawPointer) -> SparseMatrix_Float

Returns a sparse matrix of single-precision values from individual coordinate format arrays, without any internal memory allocations.

### BLAS Support

func SparseConvertFromOpaque(sparse_matrix_double) -> SparseMatrix_Double

Returns a sparse matrix of double-precision, floating-point values from a BLAS opaque matrix.

func SparseConvertFromOpaque(sparse_matrix_float) -> SparseMatrix_Float

Returns a sparse matrix of single-precision, floating-point values from a BLAS opaque matrix.

## See Also

### Creating sparse matrices

Creating sparse matrices

Create sparse matrices for factorization and solving systems.

struct SparseMatrix_Double

A structure that contains a sparse matrix of double-precision, floating-point values.

struct SparseMatrix_Float

A structure that contains a sparse matrix of single-precision, floating-point values.

