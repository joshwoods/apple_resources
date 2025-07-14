

- Accelerate
-  SparseSolve(\_:\_:\_:\_:\_:) 

Function

# SparseSolve(\_:\_:\_:\_:\_:)

Solves the equation *AX = B* for matrices of double-precision values using the specified iterative method and preconditioner type.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseSolve(
    _ method: SparseIterativeMethod,
    _ A: SparseMatrix_Double,
    _ B: DenseMatrix_Double,
    _ X: DenseMatrix_Double,
    _ Preconditioner: SparsePreconditioner_t
) -> SparseIterativeStatus_t
```

## Parameters 

`method`  

The iterative method.

`A`  

The matrix *A*.

`B`  

The matrix *B*.

`X`  

The matrix *X*.

`Preconditioner`  

The preconditioner to apply.

## Return Value

A SparseIterativeStatus_t enumeration that represents the status of the iterative solve.

## Discussion

Use this function to solve a system of linear equations using a factored coefficient matrix. Preconditioning the coefficient matrix can reduce the number of iterations the function requires to converge the system.

The following figure shows two systems of equations where the coefficient matrix is sparse:

The following code solves this system by applying a diagonal scaling preconditioner and using the least squares minimum residual method:

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

defer {
    SparseCleanup(A)
}

/// Create the right-hand-side matrix, _B_.
var bValues: [Double] = [30, 35, 100,
                         300, 350, 1000]
let n = bValues.count

let xValues = [Double](unsafeUninitializedCapacity: n) {
    buffer, count in
    bValues.withUnsafeMutableBufferPointer { bPtr in
        let B = DenseMatrix_Double(rowCount: 3,
                                   columnCount: 2,
                                   columnStride: 3,
                                   attributes: SparseAttributes_t(),
                                   data: bPtr.baseAddress!)

        let X = DenseMatrix_Double(rowCount: 3,
                                   columnCount: 2,
                                   columnStride: 3,
                                   attributes: SparseAttributes_t(),
                                   data: buffer.baseAddress!)

        SparseSolve(SparseLSMR(),
                    A, B, X,
                    SparsePreconditionerDiagScaling)
        count = n
    }
}
```

On return, x`Values` contains the values `[1.0, 2.0, 3.0, 10.0, 20.0, 30.0]`.

## See Also

### Iterative Sparse Solve Functions with Preconditioner

func SparseSolve(SparseIterativeMethod, SparseMatrix_Double, DenseMatrix_Double, DenseMatrix_Double, SparseOpaquePreconditioner_Double) -> SparseIterativeStatus_t

Solves the equation *AX = B* for matrices of double-precision values using the specified iterative method and opaque preconditioner.

func SparseSolve(SparseIterativeMethod, SparseMatrix_Float, DenseMatrix_Float, DenseMatrix_Float, SparseOpaquePreconditioner_Float) -> SparseIterativeStatus_t

Solves the equation *AX = B* for matrices of single-precision values using the specified iterative method and opaque preconditioner.

func SparseSolve(SparseIterativeMethod, SparseMatrix_Float, DenseMatrix_Float, DenseMatrix_Float, SparsePreconditioner_t) -> SparseIterativeStatus_t

Solves the equation *AX = B* for matrices of single-precision values using the specified iterative method and preconditioner type.

func SparseSolve(SparseIterativeMethod, (Bool, CBLAS_TRANSPOSE, DenseMatrix_Double, DenseMatrix_Double) -> Void, DenseMatrix_Double, DenseMatrix_Double, SparseOpaquePreconditioner_Double) -> SparseIterativeStatus_t

Solves the equation *AX = B* for matrices of double-precision values, treating *A* as an operator and using the specified iterative method.

func SparseSolve(SparseIterativeMethod, (Bool, CBLAS_TRANSPOSE, DenseMatrix_Float, DenseMatrix_Float) -> Void, DenseMatrix_Float, DenseMatrix_Float, SparseOpaquePreconditioner_Float) -> SparseIterativeStatus_t

Solves the equation *AX = B* for matrices of single-precision values, treating *A* as an operator and using the specified iterative method.

