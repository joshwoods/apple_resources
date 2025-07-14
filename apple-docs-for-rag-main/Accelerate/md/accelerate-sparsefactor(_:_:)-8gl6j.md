

- Accelerate
-  SparseFactor(\_:\_:) 

Function

# SparseFactor(\_:\_:)

Returns the specified factorization of a sparse matrix of double-precision values.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseFactor(
    _ type: SparseFactorization_t,
    _ Matrix: SparseMatrix_Double
) -> SparseOpaqueFactorization_Double
```

## Parameters 

`type`  

The type of factorization to perform.

`Matrix`  

The matrix to factorize.

## Return Value

A SparseOpaqueFactorization_Double structure that represents the matrix factorization.

## Mentioned in 

Solving systems using direct methods

## Discussion

Use this function to calculate the factorization of a sparse matrix to pass to the direct solve functions. The following figure shows a system of equations where the coefficient matrix is sparse:

The following code solves this system with a QR factorization of the coefficient matrix:

```
/// Create the coefficient matrix _A_.
let rowIndices: [Int32] =    [ 0,  1, 1,  2]
let columnIndices: [Int32] = [ 2,  0, 2,  1]
let aValues: [Double] =      [10, 20, 5, 50]

let A = SparseConvertFromCoordinate(3, 3,
                                    4, 1,
                                    SparseAttributes_t(),
                                    rowIndices, columnIndices,
                                    aValues)

/// Factorize _A_.
let factorization = SparseFactor(SparseFactorizationQR, A)

defer {
    SparseCleanup(A)
    SparseCleanup(factorization)
}

/// Create the right-hand-side vector, _b_.
var bValues = [30.0, 35.0, 100.0]

bValues.withUnsafeMutableBufferPointer { bPtr in

    let xb = DenseVector_Double(count: 3,
                               data: bPtr.baseAddress!)

    SparseSolve(factorization, xb)
}
```

On return, `bValues` contains the values `[1.0, 2.0, 3.0]`.

You can use the symbolic factorization that this function returns for multiple numerical factorizations with different numerical values but the same nonzero structure.

## See Also

### Matrix Factorization Functions

func SparseFactor(SparseFactorization_t, SparseMatrix_Float) -> SparseOpaqueFactorization_Float

Returns the specified factorization of a sparse matrix of single-precision values.

func SparseFactor(SparseFactorization_t, SparseMatrix_Double, SparseSymbolicFactorOptions, SparseNumericFactorOptions) -> SparseOpaqueFactorization_Double

Returns the specified factorization of a sparse matrix of double-precision values using the specified options.

func SparseFactor(SparseFactorization_t, SparseMatrix_Float, SparseSymbolicFactorOptions, SparseNumericFactorOptions) -> SparseOpaqueFactorization_Float

Returns the specified factorization of a sparse matrix of single-precision values using the specified options.

