

- Accelerate
-  SparseSolve(\_:\_:\_:\_:\_:) 

Function

# SparseSolve(\_:\_:\_:\_:\_:)

Solves the equation *Ax = b* for vectors of single-precision values using the specified iterative method and preconditioner type.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseSolve(
    _ method: SparseIterativeMethod,
    _ A: SparseMatrix_Float,
    _ b: DenseVector_Float,
    _ x: DenseVector_Float,
    _ Preconditioner: SparsePreconditioner_t
) -> SparseIterativeStatus_t
```

## Parameters 

`method`  

The iterative method.

`A`  

The matrix *A*.

`b`  

The vector *b*.

`x`  

The vector *x*.

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
let aValues: [Float] =       [10, 20, 5, 50]

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

bValues.withUnsafeMutableBufferPointer { bPtr in
    xValues.withUnsafeMutableBufferPointer { xPtr in

        let b = DenseVector_Float(count: 3,
                                  data: bPtr.baseAddress!)

        let x = DenseVector_Float(count: 3,
                                  data: xPtr.baseAddress!)

        SparseSolve(SparseLSMR(),
                    A, b, x,
                    SparsePreconditionerDiagScaling)
    }
}
```

On return, x`Values` contains the values `[1.0, 2.0, 3.0]`.

## See Also

### Iterative Sparse Solve Functions with Preconditioner

func SparseSolve(SparseIterativeMethod, SparseMatrix_Double, DenseVector_Double, DenseVector_Double, SparseOpaquePreconditioner_Double) -> SparseIterativeStatus_t

Solves the equation *Ax = b* for vectors of double-precision values using the specified iterative method and opaque preconditioner.

func SparseSolve(SparseIterativeMethod, SparseMatrix_Float, DenseVector_Float, DenseVector_Float, SparseOpaquePreconditioner_Float) -> SparseIterativeStatus_t

Solves the equation *Ax = b* for vectors of single-precision values using the specified iterative method and opaque preconditioner.

func SparseSolve(SparseIterativeMethod, SparseMatrix_Double, DenseVector_Double, DenseVector_Double, SparsePreconditioner_t) -> SparseIterativeStatus_t

Solves the equation *Ax = b* for vectors of double-precision values using the specified iterative method and preconditioner type.

func SparseSolve(SparseIterativeMethod, (Bool, CBLAS_TRANSPOSE, DenseVector_Double, DenseVector_Double) -> Void, DenseVector_Double, DenseVector_Double, SparseOpaquePreconditioner_Double) -> SparseIterativeStatus_t

Solves the equation *Ax = b* for vectors of double-precision values, treating *A* as an operator and using the specified iterative method and preconditioner.

func SparseSolve(SparseIterativeMethod, (Bool, CBLAS_TRANSPOSE, DenseVector_Float, DenseVector_Float) -> Void, DenseVector_Float, DenseVector_Float, SparseOpaquePreconditioner_Float) -> SparseIterativeStatus_t

Solves the equation *Ax = b* for vectors of single-precision values, treating *A* as an operator and using the specified iterative method and preconditioner.

