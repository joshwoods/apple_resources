

- Accelerate
-  SparseSolve(\_:\_:\_:) 

Function

# SparseSolve(\_:\_:\_:)

Solves the system *Ax = b* using the supplied double-precision factorization of *A*.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseSolve(
    _ Factored: SparseOpaqueFactorization_Double,
    _ b: DenseVector_Double,
    _ x: DenseVector_Double
)
```

## Parameters 

`Factored`  

The factored matrix to solve.

`b`  

The vector *b*.

`x`  

The vector x.

## Mentioned in 

Solving systems using direct methods

## Discussion

Use this function to solve a system of linear equations using a factored coefficient matrix. The following figure shows a system of equations where the coefficient matrix is sparse:

The following code solves this system with a QR factorization of the coefficient matrix:

```
/// Create the coefficient matrix _A.
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
var bValues: [Double] = [30, 35, 100]
let n = bValues.count

/// Solve the system.
let xValues = [Double](unsafeUninitializedCapacity: n) {
    buffer, count in

    bValues.withUnsafeMutableBufferPointer { bPtr in

        let b = DenseVector_Double(count: 3,
                                   data: bPtr.baseAddress!)
        let x = DenseVector_Double(count: 3,
                                   data: buffer.baseAddress!)

        SparseSolve(factorization, b, x)

        count = n
    }
}
```

On return, x`Values` contains the values `[1.0, 2.0, 3.0]`.

If the factorization is *A = QR*, the function returns the solution of minimum norm *‖ x ‖₂* for underdetermined systems.

If the factorization is *A = QR*, the function returns the least squares solution *minₓ ‖ AX - B ‖₂* for overdetermined systems.

If the factorization is SparseFactorizationCholeskyAtA, the factorization is of *AᵀA*, and the solution that returns is for the system *AᵀAX = B*.

## See Also

### Out-of-Place Direct Solving Functions

func SparseSolve(SparseOpaqueFactorization_Float, DenseVector_Float, DenseVector_Float)

Solves the system *Ax = b* using the supplied single-precision factorization of *A*.

