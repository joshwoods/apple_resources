

- Accelerate
-  SparseSolve(\_:\_:\_:\_:) 

Function

# SparseSolve(\_:\_:\_:\_:)

Solves the equation *AX = B* for matrices of single-precision values, treating *A* as an operator and using the specified iterative method.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseSolve(
    _ method: SparseIterativeMethod,
    _ ApplyOperator: @escaping (Bool, CBLAS_TRANSPOSE, DenseMatrix_Float, DenseMatrix_Float) -> Void,
    _ B: DenseMatrix_Float,
    _ X: DenseMatrix_Float
) -> SparseIterativeStatus_t
```

## Parameters 

`method`  

The iterative method.

`ApplyOperator`  

The apply operator block to run. The block takes the following parameters:

accumulate  
Indicates whether to perform `Y += op(A)X` (if `true`), or `Y = op(A)X` (if `false`).

trans  
Indicates whether `op(A)` is the application of *A* if `CblasNoTrans`, or *Aᵀ* if `CblasTrans`

X  
The matrix to multiply.

Y  
The matrix for accumulating or storing the result.

`B`  

The matrix *B*.

`X`  

The matrix *X*.

## Return Value

A SparseIterativeStatus_t enumeration that represents the status of the iterative solve.

## Discussion

Use this function to solve a system of linear equations using a factored coefficient matrix. In cases where the matrix *A* isn’t explicitly available or you need control over the multiplication, this function allows you to provide an apply block.

The following figure shows two systems of equations where the coefficient matrix is sparse:

The following code solves this system using the least squares minimum residual method:

```
let rowIndices: [Int32] =    [ 0,  1, 1,  2]
let columnIndices: [Int32] = [ 2,  0, 2,  1]
let aValues: [Float] =       [10, 20, 5, 50]

let A = SparseConvertFromCoordinate(3, 3,
                                    4, 1,
                                    SparseAttributes_t(),
                                    rowIndices, columnIndices,
                                    aValues)

defer {
    SparseCleanup(A)
}

/// Create the right-hand-side matrix, _B_.
var bValues: [Float] = [30, 35, 100,
                        300, 350, 1000]

var xValues: [Float] = [0, 0, 0,
                        0, 0, 0]

/// Create the apply operator block.
func applyOperator(accumulate: Bool,
                   trans: CBLAS_TRANSPOSE,
                   X: DenseMatrix_Float,
                   Y: DenseMatrix_Float) {
    switch(accumulate, trans == CblasTrans) {
        case (false, false):
            SparseMultiply(A, X, Y)
        case (false, true):
            SparseMultiply(SparseGetTranspose(A), X, Y)
        case (true, false):
            SparseMultiplyAdd(A, X, Y)
        case (true, true):
            SparseMultiplyAdd(SparseGetTranspose(A), X, Y)
    }
}

xValues.withUnsafeMutableBufferPointer { xPtr in
    bValues.withUnsafeMutableBufferPointer { bPtr in
        let B = DenseMatrix_Float(rowCount: 3,
                                  columnCount: 2,
                                  columnStride: 3,
                                  attributes: SparseAttributes_t(),
                                  data: bPtr.baseAddress!)

        let X = DenseMatrix_Float(rowCount: 3,
                                  columnCount: 2,
                                  columnStride: 3,
                                  attributes: SparseAttributes_t(),
                                  data: xPtr.baseAddress!)

        SparseSolve(SparseLSMR(),
                    applyOperator,
                    B, X)
    }
}
```

On return, x`Values` contains the values `[1.0, 2.0, 3.0, 10.0, 20.0, 30.0]`.

## See Also

### Iterative Sparse Solve Functions

func SparseSolve(SparseIterativeMethod, SparseMatrix_Double, DenseMatrix_Double, DenseMatrix_Double) -> SparseIterativeStatus_t

Solves the equation *AX = B* for matrices of double-precision values using the specified iterative method.

func SparseSolve(SparseIterativeMethod, SparseMatrix_Float, DenseMatrix_Float, DenseMatrix_Float) -> SparseIterativeStatus_t

Solves the equation *AX = B* for matrices of single-precision values using the specified iterative method.

func SparseSolve(SparseIterativeMethod, (Bool, CBLAS_TRANSPOSE, DenseMatrix_Double, DenseMatrix_Double) -> Void, DenseMatrix_Double, DenseMatrix_Double) -> SparseIterativeStatus_t

Solves the equation *AX = B* for matrices of double-precision values, treating *A* as an operator and using the specified iterative method.

