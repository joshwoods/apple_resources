

- Accelerate
-  SparseSolve(\_:\_:) 

Function

# SparseSolve(\_:\_:)

Solves the system *Ax = b* using the supplied single-precision factorization of *A*, in place.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseSolve(
    _ Factored: SparseOpaqueFactorization_Float,
    _ xb: DenseVector_Float
)
```

## Parameters 

`Factored`  

The factored matrix to solve.

`xb`  

On input, the vector *b*. On return, the function overwrites with the vector *x*. If *A* has dimension *m x n*, this parameter must have length *k*, where *k = max(m,n)*.

## Discussion

Use this function to solve a system of linear equations using a factored coefficient matrix. The following figure shows a system of equations where the coefficient matrix is sparse:

The following code solves this system with a QR factorization of the coefficient matrix:

```
/// Create the coefficient matrix _A_.
let rowIndices: [Int32] =    [ 0,  1, 1,  2]
let columnIndices: [Int32] = [ 2,  0, 2,  1]
let aValues: [Float] =       [10, 20, 5, 50]

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
var bValues: [Float] = [30, 35, 100]

/// Solve the system.
bValues.withUnsafeMutableBufferPointer { bPtr in
    let xb = DenseVector_Float(count: 3,
                               data: bPtr.baseAddress!)

    SparseSolve(factorization, xb)
}
```

On return, `bValues` contains the values `[1.0, 2.0, 3.0]`.

If the factorization is *A = QR*, the function returns the solution of minimum norm *‖ x ‖₂* for underdetermined systems.

If the factorization is *A = QR*, the function returns the least squares solution *minₓ ‖ AX - B ‖₂* for overdetermined systems.

If the factorization is SparseFactorizationCholeskyAtA, the factorization is of *AᵀA*, and the solution that returns is for the system *AᵀAX = B*.

## See Also

### In-Place Direct Solving Functions

func SparseSolve(SparseOpaqueFactorization_Double, DenseVector_Double)

Solves the system *Ax = x* using the supplied double-precision factorization of *A*.

