

- Accelerate
-  SparseRefactor(\_:\_:) 

Function

# SparseRefactor(\_:\_:)

Computes a factorization of the specified double-precision matrix using an existing factorization’s storage.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseRefactor(
    _ Matrix: SparseMatrix_Double,
    _ Factorization: UnsafeMutablePointer
)
```

## Parameters 

`Matrix`  

The matrix that contains numerical data to recompute.

`Factorization`  

On input, the factorization to recompute. On output, the recomputed result.

## Discussion

Use this function to calculate the factorization of a sparse matrix to pass to the direct solve functions using an existing factorization’s storage. The specified matrix must have the same sparsity structure as the matrix of the original factorization.

This function provides behavior similar to SparseFactor(_:_:_:_:_:) by reusing explicit storage that you supply to SparseFactor(_:_:_:_:_:) as the argument `factorStorage`. However, in addition to providing a simplified call sequence, this call can also reuse any additional storage that you allocate to accommodate delayed pivots.

The following figure shows two systems of equations where the coefficient matrix is sparse:

The following code solves these two systems with refactoring. After factorizing and solving for the coefficient matrix *A0*, the code refactors and solves for matrix *A1*.

```
/// Define the sparsity structure of matrices `A0` and `A1`.
let rowIndices: [Int32] =    [ 0, 1, 1, 2]
let columnIndices: [Int32] = [ 2, 0, 2, 1]

/// Create the single-precision coefficient matrix _A0_.
let a0Values: [Double] = [10, 20, 5, 50]
let A0 = SparseConvertFromCoordinate(3, 3,
                                     4, 1,
                                     SparseAttributes_t(),
                                     rowIndices, columnIndices,
                                     a0Values)

/// Factorize _A0_.
var factorization = SparseFactor(SparseFactorizationQR, A0)

/// Solve _A0 · x = b0_ in place.
var b0Values: [Double] = [30, 35, 100]
b0Values.withUnsafeMutableBufferPointer { bPtr in
    let xb = DenseVector_Double(count: 3,
                               data: bPtr.baseAddress!)

    SparseSolve(factorization, xb)
}

/// Create the double-precision coefficient matrix _A1_.
let a1Values: [Double] = [5, 10, 2.5, 25]
let A1 = SparseConvertFromCoordinate(3, 3,
                                     4, 1,
                                     SparseAttributes_t(),
                                     rowIndices, columnIndices,
                                     a1Values)

/// Factorize _A1_ into the existing factorization.
SparseRefactor(A1, &factorization)

/// Solve _A1 · x = b1_ in place.
var b1Values: [Double] = [60, 70, 200]
b1Values.withUnsafeMutableBufferPointer { bPtr in
    let xb = DenseVector_Double(count: 3,
                                data: bPtr.baseAddress!)

    SparseSolve(factorization, xb)
}

SparseCleanup(A0)
SparseCleanup(A1)
SparseCleanup(factorization)
```

On return, `b0Values` contains the values `[1.0, 2.0, 3.0]`, and `b1Values` contains the values `[4.0, 8.0, 12.0]`.

## See Also

### Matrix Refactorization Functions

func SparseRefactor(SparseMatrix_Float, UnsafeMutablePointer&lt;SparseOpaqueFactorization_Float>)

Computes a factorization of the specified single-precision matrix using an existing factorization’s storage.

func SparseRefactor(SparseMatrix_Double, UnsafeMutablePointer&lt;SparseOpaqueFactorization_Double>, SparseNumericFactorOptions)

Computes a factorization of the specified double-precision matrix using an existing factorization’s storage and specified options.

func SparseRefactor(SparseMatrix_Float, UnsafeMutablePointer&lt;SparseOpaqueFactorization_Float>, SparseNumericFactorOptions)

Computes a factorization of the specified single-precision matrix using an existing factorization’s storage and specified options.

