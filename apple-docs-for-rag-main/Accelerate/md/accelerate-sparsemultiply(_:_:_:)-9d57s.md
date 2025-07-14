

- Accelerate
-  SparseMultiply(\_:\_:\_:) 

Function

# SparseMultiply(\_:\_:\_:)

Performs the multiplication *y = Ax* on a vector of double-precision, floating-point values.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseMultiply(
    _ A: SparseMatrix_Double,
    _ x: DenseVector_Double,
    _ y: DenseVector_Double
)
```

## Parameters 

`A`  

The sparse matrix *A* in *y* *= Ax*.

`x`  

The dense vector *x* in *y* *= Ax*.

`y`  

The dense vector *y* in *y* *= Ax*.

## Discussion

Use this function to multiply a sparse matrix by a dense vector. The following equation is an example of a matrix-vector multiplication where the matrix is sparse:

Call SparseMultiply(_:_:_:) to calculate the result.

```
let rowCount = Int32(4)
let columnCount = Int32(4)
let blockCount = 4
let blockSize = UInt8(1)
let rowIndices: [Int32] = [0, 3, 0, 3]
let columnIndices: [Int32] = [0, 0, 3, 3]
let data = [1.0, 4.0, 13.0, 16.0]

/// The _A_ in _y=Ax_.
let A = SparseConvertFromCoordinate(rowCount, columnCount,
                                    blockCount, blockSize,
                                    SparseAttributes_t(),
                                    rowIndices, columnIndices,
                                    data)
defer {
    SparseCleanup(A)
}

/// The values for _x_ in _y=Ax_.
var xValues = [10.0, -1.0, -1.0, 10.0]

/// The values for _y_ in _y=Ax_.
let yValues = [Double](unsafeUninitializedCapacity: xValues.count) {
    resultBuffer, count in

    xValues.withUnsafeMutableBufferPointer { xValuesPtr in
        /// The _x_ in _y=Ax_.
        let x = DenseVector_Double(count: 4, 
                                   data: xValuesPtr.baseAddress!)

        /// The _y_ in _y=Ax_.
        let y = DenseVector_Double(count: 4,
                                   data: resultBuffer.baseAddress!)

        SparseMultiply(A, x, y)
    }

    count = xValues.count
}

/// On return, `yValues` contains:
///      `[ 140.0, 0.0, 0.0,  200.0 ]`
```

## See Also

### Multiplication Functions

func SparseMultiply(SparseMatrix_Float, DenseVector_Float, DenseVector_Float)

Performs the multiplication *y = Ax* on a vector of single-precision, floating-point values.

func SparseMultiply(Double, SparseMatrix_Double, DenseVector_Double, DenseVector_Double)

Performs the multiply operation *y* *= alpha \* Ax* on a vector of double-precision, floating-point values.

func SparseMultiply(Float, SparseMatrix_Float, DenseVector_Float, DenseVector_Float)

Performs the multiply operation *y* *= alpha \* Ax* on a vector of single-precision, floating-point values.

