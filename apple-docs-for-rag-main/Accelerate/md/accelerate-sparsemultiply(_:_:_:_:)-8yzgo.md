

- Accelerate
-  SparseMultiply(\_:\_:\_:\_:) 

Function

# SparseMultiply(\_:\_:\_:\_:)

Performs the multiply operation *y* *= alpha \* Ax* on a vector of single-precision, floating-point values.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseMultiply(
    _ alpha: Float,
    _ A: SparseMatrix_Float,
    _ x: DenseVector_Float,
    _ y: DenseVector_Float
)
```

## Parameters 

`alpha`  

The scalar value *alpha* in *y* *= alpha \* Ax*.

`A`  

The sparse matrix *A* in *y* *= Ax*.

`x`  

The dense vector *x* in *y* *= Ax*.

`y`  

The dense vector *y* in *y* *= Ax*.

## Discussion

Use this function to multiply a scalar by a sparse matrix, and then by a dense vector. The following equation is an example of a scalar-matrix-vector multiplication where the matrix is sparse:

Call SparseMultiply(_:_:_:_:) to calculate the result.

```
let rowCount = Int32(4)
let columnCount = Int32(4)
let blockCount = 4
let blockSize = UInt8(1)
let rowIndices: [Int32] = [0, 3, 0, 3]
let columnIndices: [Int32] = [0, 0, 3, 3]
let data: [Float] = [1.0, 4.0, 13.0, 16.0]

/// The _A_ in _y = alpha * Ax_.
let A = SparseConvertFromCoordinate(rowCount, columnCount,
                                    blockCount, blockSize,
                                    SparseAttributes_t(),
                                    rowIndices, columnIndices,
                                    data)
defer {
    SparseCleanup(A)
}

/// The values for _x_ in _y = alpha * Ax_.
var xValues: [Float] = [10.0, -1.0, -1.0, 10.0]

let alpha: Float = 2.0

/// The values for _y_ in _y = alpha * Ax_.
let yValues = [Float](unsafeUninitializedCapacity: xValues.count) {
    resultBuffer, count in

    xValues.withUnsafeMutableBufferPointer { xValuesPtr in
        /// The _x_ in _y = alpha * Ax_.
        let x = DenseVector_Float(count: 4, 
                                  data: xValuesPtr.baseAddress!)

        /// The _y_ in _y = alpha * Ax_.
        let y = DenseVector_Float(count: 4,
                                  data: resultBuffer.baseAddress!)

        SparseMultiply(alpha, A, x, y)
    }

    count = xValues.count
}

/// On return, `yValues` contains:
///      `[ 280.0, 0.0, 0.0,  400.0 ]`
```

## See Also

### Multiplication Functions

func SparseMultiply(SparseMatrix_Double, DenseVector_Double, DenseVector_Double)

Performs the multiplication *y = Ax* on a vector of double-precision, floating-point values.

func SparseMultiply(SparseMatrix_Float, DenseVector_Float, DenseVector_Float)

Performs the multiplication *y = Ax* on a vector of single-precision, floating-point values.

func SparseMultiply(Double, SparseMatrix_Double, DenseVector_Double, DenseVector_Double)

Performs the multiply operation *y* *= alpha \* Ax* on a vector of double-precision, floating-point values.

