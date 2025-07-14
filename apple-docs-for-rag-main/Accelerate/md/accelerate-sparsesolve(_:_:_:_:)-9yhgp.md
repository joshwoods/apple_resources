

- Accelerate
-  SparseSolve(\_:\_:\_:\_:) 

Function

# SparseSolve(\_:\_:\_:\_:)

Solves the equation *Ax = b* for vectors of single-precision values, treating *A* as an operator and using the specified iterative method.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseSolve(
    _ method: SparseIterativeMethod,
    _ ApplyOperator: @escaping (Bool, CBLAS_TRANSPOSE, DenseVector_Float, DenseVector_Float) -> Void,
    _ b: DenseVector_Float,
    _ x: DenseVector_Float
) -> SparseIterativeStatus_t
```

## Parameters 

`method`  

The iterative method.

`ApplyOperator`  

The apply operator block to run. The block takes the following parameters:

accumulate  
Indicates whether to perform `y` `+= op(A)`x (if `true`), or `Y = op(A)X` (if `false`).

trans  
Indicates whether `op(A)` is the application of *A* if `CblasNoTrans`, or *Aᵀ* if `CblasTrans`

x  
The vector to multiply.

y  
The vector for accumulating or storing the result.

`b`  

The vector *b*.

`x`  

The matrix *x*.

## Return Value

A SparseIterativeStatus_t enumeration that represents the status of the iterative solve.

## Discussion

Use this function to solve a system of linear equations using a factored coefficient matrix. In cases where the matrix *A* isn’t explicitly available or you need control over the multiplication, this function allows you to provide an apply block.

The following figure shows two systems of equations where the coefficient matrix is sparse:

The following code solves this system using the least squares minimum residual method:

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
defer {
    SparseCleanup(A)
}

/// Create the right-hand-side vector, _b_.
var bValues: [Float] = [30, 35, 100]
var xValues = [Float](repeating: .nan, count: bValues.count)

/// Create the apply operator block.
func applyOperator(accumulate: Bool,
                   trans: CBLAS_TRANSPOSE,
                   x: DenseVector_Float,
                   y: DenseVector_Float) {

    switch(accumulate, trans == CblasTrans) {
        case (false, false):
            SparseMultiply(A, x, y)
        case (false, true):
            SparseMultiply(SparseGetTranspose(A), x, y)
        case (true, false):
            SparseMultiplyAdd(A, x, y)
        case (true, true):
            SparseMultiplyAdd(SparseGetTranspose(A), x, y)
    }
}

bValues.withUnsafeMutableBufferPointer { bPtr in
    xValues.withUnsafeMutableBufferPointer { xPtr in

        let b = DenseVector_Float(count: 3,
                                  data: bPtr.baseAddress!)

        let x = DenseVector_Float(count: 3,
                                  data: xPtr.baseAddress!)

        SparseSolve(SparseLSMR(),
                    applyOperator,
                    b, x)
    }
}
```

On return, x`Values` contains the values `[1.0, 2.0, 3.0]`.

## See Also

### Iterative Sparse Solve Functions

func SparseSolve(SparseIterativeMethod, SparseMatrix_Double, DenseVector_Double, DenseVector_Double) -> SparseIterativeStatus_t

Solves the equation *Ax = b* for vectors of double-precision values using the specified iterative method.

func SparseSolve(SparseIterativeMethod, SparseMatrix_Float, DenseVector_Float, DenseVector_Float) -> SparseIterativeStatus_t

Solves the equation *Ax = b* for vectors of single-precision values using the specified iterative method.

func SparseSolve(SparseIterativeMethod, (Bool, CBLAS_TRANSPOSE, DenseVector_Double, DenseVector_Double) -> Void, DenseVector_Double, DenseVector_Double) -> SparseIterativeStatus_t

Solves the equation *Ax = b* for vectors of double-precision values, treating *A* as an operator and using the specified iterative method.

