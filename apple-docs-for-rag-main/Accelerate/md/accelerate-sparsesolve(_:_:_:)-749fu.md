

- Accelerate
-  SparseSolve(\_:\_:\_:) 

Function

# SparseSolve(\_:\_:\_:)

Solves the system *AX = B* using the supplied single-precision factorization of *A*, in place and without any internal memory allocations.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseSolve(
    _ Factored: SparseOpaqueFactorization_Float,
    _ XB: DenseMatrix_Float,
    _ workspace: UnsafeMutableRawPointer
)
```

## Parameters 

`Factored`  

The factorization of *A*.

`XB`  

On entry, the right-hand-side, *B*. On return, the solution vectors *X*. If *A* has dimension *m x n*, *XB* must have dimension *k x nrhs*, where *k = max(m,n)* and *nrhs* is the number of right-hand-sides to find solutions for.

`workspace`  

The scratch space of size solveWorkspaceRequiredStatic `+` `nrhs` `*` solveWorkspaceRequiredPerRHS.

## Discussion

Use this function to solve a system of linear equations using a factored coefficient matrix. In cases where your code calls the function frequently, create and manage the workspace that the Sparse Solvers library uses and reuse it across function calls. Reusing a workspace prevents the Sparse Solvers library from allocating the temporary storage with each call.

The following figure shows two systems of equations where the coefficient matrix is sparse:

The following code solves this system with a QR factorization of the coefficient matrix:

```
/// Create the coefficient matrix _A_.
let rowIndices: [Int32] =    [ 0,  1, 1,  2]
let columnIndices: [Int32] = [ 2,  0, 2,  1]
let aValues: [Float] =      [10, 20, 5, 50]

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

/// Create the workspace.
let nrhs = Int(A.structure.columnCount)
let byteCount = factorization.solveWorkspaceRequiredStatic +
                    nrhs * factorization.solveWorkspaceRequiredPerRHS
let workspace = UnsafeMutableRawPointer.allocate(
    byteCount: byteCount,
    alignment: MemoryLayout.alignment)
defer {
    workspace.deallocate()
}

/// Create the right-hand-side matrix, _B_.
var bValues: [Float] = [30, 35, 100,
                        300, 350, 1000]

/// Solve the system.
bValues.withUnsafeMutableBufferPointer { bPtr in
    let XB = DenseMatrix_Float(rowCount: 3,
                               columnCount: 2,
                               columnStride: 3,
                               attributes: SparseAttributes_t(),
                               data: bPtr.baseAddress!)

    SparseSolve(factorization, XB,
                workspace)
}
```

On return, `bValues` contains the values `[1.0, 2.0, 3.0, 10.0, 20.0, 30.0]`.

If the factorization is *A = QR*, the function returns the solution of minimum norm *‖ x ‖₂* for underdetermined systems.

If the factorization is *A = QR*, the function returns the least squares solution *minₓ ‖ AX - B ‖₂* for overdetermined systems.

If the factorization is SparseFactorizationCholeskyAtA, the factorization is of *AᵀA*, and the solution that returns is for the system *AᵀAX = B*.

## See Also

### In-Place Direct Solving Functions with User-Defined Workspace

func SparseSolve(SparseOpaqueFactorization_Double, DenseMatrix_Double, UnsafeMutableRawPointer)

Solves the system *AX = B* using the supplied double-precision factorization of *A*, in place and without any internal memory allocations.

