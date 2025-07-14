

- Accelerate
-  SparseFactor(\_:\_:\_:) 

Function

# SparseFactor(\_:\_:\_:)

Returns the factorization of a sparse matrix of single-precision values that corresponds to the supplied symbolic factorization using specified options.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseFactor(
    _ SymbolicFactor: SparseOpaqueSymbolicFactorization,
    _ Matrix: SparseMatrix_Float,
    _ nfoptions: SparseNumericFactorOptions
) -> SparseOpaqueFactorization_Float
```

## Parameters 

`SymbolicFactor`  

A symbolic factorization that returns by calling SparseFactor(_:_:_:_:_:).

`Matrix`  

The matrix to factorize.

`nfoptions`  

The numeric factor options, such as pivoting parameters.

## Return Value

A SparseOpaqueFactorization_Float structure that represents the matrix factorization.

## Discussion

Use this function to solve a system of linear equations using a symbolic factorization that SparseFactor(_:_:) creates.

The following figure shows two systems of equations where the coefficient matrix is sparse:

The following code solves these two systems by calling SparseFactor(_:_:) and SparseFactor(_:_:):

```
/// Define the sparsity pattern of matrices `A0` and `A1`.
let rowIndices: [Int32] =    [ 0, 1, 1, 2]
let columnIndices: [Int32] = [ 2, 0, 2, 1]

/// Create the single-precision coefficient matrix _A0_.
let a0Values: [Float] = [10, 20, 5, 50]
let A0 = SparseConvertFromCoordinate(3, 3,
                                     4, 1,
                                     SparseAttributes_t(),
                                     rowIndices, columnIndices,
                                     a0Values)

/// Create the double-precision coefficient matrix _A1_.
let a1Values: [Double] = [5, 10, 2.5, 25]
let A1 = SparseConvertFromCoordinate(3, 3,
                                     4, 1,
                                     SparseAttributes_t(),
                                     rowIndices, columnIndices,
                                     a1Values)

/// Compute the symbolic factorization from the structure of either coefficient matrix.
let structure = A0.structure
let symbolicFactorization = SparseFactor(SparseFactorizationQR,
                                         structure)

/// Factorize _A0_ using the symbolic factorization.
let factorization0 = SparseFactor(symbolicFactorization, A0)

/// Solve _A0 · x = b0_ in place.
var b0Values: [Float] = [30, 35, 100]
b0Values.withUnsafeMutableBufferPointer { bPtr in
    let xb = DenseVector_Float(count: 3,
                               data: bPtr.baseAddress!)

    SparseSolve(factorization0, xb)
}

/// Factorize _A1_ using the symbolic factorization.
let factorization1 = SparseFactor(symbolicFactorization, A1)

/// Solve _A1 · x = b1_ in place.
var b1Values: [Double] = [60, 70, 200]
b1Values.withUnsafeMutableBufferPointer { bPtr in
    let xb = DenseVector_Double(count: 3,
                               data: bPtr.baseAddress!)

    SparseSolve(factorization1, xb)
}

SparseCleanup(A0)
SparseCleanup(A1)
SparseCleanup(factorization0)
SparseCleanup(factorization1)
```

On return, `b0Values` contains the values `[1.0, 2.0, 3.0]`, and `b1Values` contains the values `[4.0, 8.0, 12.0]`.

## See Also

### Related Documentation

func SparseFactor(SparseFactorization_t, SparseMatrixStructure) -> SparseOpaqueSymbolicFactorization

Returns a symbolic factorization of the requested type for a specified sparsity structure.

### Matrix Factorizations Using Precalculated Symbolic Factorization

func SparseFactor(SparseOpaqueSymbolicFactorization, SparseMatrix_Double) -> SparseOpaqueFactorization_Double

Returns the factorization of a sparse matrix of double-precision values that corresponds to the supplied symbolic factorization.

func SparseFactor(SparseOpaqueSymbolicFactorization, SparseMatrix_Float) -> SparseOpaqueFactorization_Float

Returns the factorization of a sparse matrix of single-precision values that corresponds to the supplied symbolic factorization.

func SparseFactor(SparseOpaqueSymbolicFactorization, SparseMatrix_Double, SparseNumericFactorOptions) -> SparseOpaqueFactorization_Double

Returns the factorization of a sparse matrix of double-precision values that corresponds to the supplied symbolic factorization using specified options.

