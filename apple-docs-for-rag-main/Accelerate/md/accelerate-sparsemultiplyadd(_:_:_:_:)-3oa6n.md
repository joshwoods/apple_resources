

- Accelerate
-  SparseMultiplyAdd(\_:\_:\_:\_:) 

Function

# SparseMultiplyAdd(\_:\_:\_:\_:)

Performs the multiply operation *y += alpha \* Ax* on a vector of double-precision, floating-point values.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseMultiplyAdd(
    _ alpha: Double,
    _ A: SparseMatrix_Double,
    _ x: DenseVector_Double,
    _ y: DenseVector_Double
)
```

## Parameters 

`alpha`  

The scalar value *alpha* in *y* *+= alpha \* Ax*.

`A`  

The sparse matrix *A* in *y* *+= Ax*.

`x`  

The dense vector *x* in *y* *+= Ax*.

`y`  

The dense vector *y* in *y* *+= Ax*.

## Discussion

Use this function to multiply a scalar by a sparse matrix, then by a dense vector, and accumulate the result. The following equation is an example of a matrix-vector multiplication where the matrix is sparse:

Call SparseMultiplyAdd(_:_:_:_:) to calculate the result.

```
let rowCount = Int32(4)
let columnCount = Int32(4)
let blockCount = 4
let blockSize = UInt8(1)
let rowIndices: [Int32] = [0, 3, 0, 3]
let columnIndices: [Int32] = [0, 0, 3, 3]
let data = [1.0, 4.0, 13.0, 16.0]

/// The _A_ in _y+=Ax_.
let A = SparseConvertFromCoordinate(rowCount, columnCount,
                                    blockCount, blockSize,
                                    SparseAttributes_t(),
                                    rowIndices, columnIndices,
                                    data)
defer {
    SparseCleanup(A)
}

/// The values for _x_ in _y+=Ax_.
var xValues = [10.0, -1.0, -1.0, 10.0]

var yValues = [1.0, 1.0, 1.0, 1.0]

let alpha = 2.0

/// The values for _y_ in _y+=Ax_.
yValues.withUnsafeMutableBufferPointer { yValuesPtr in

    xValues.withUnsafeMutableBufferPointer { xValuesPtr in
        /// The _x_ in _y+=Ax_.
        let x = DenseVector_Double(count: 4,
                                   data: xValuesPtr.baseAddress!)

        /// The _y_ in _y+=Ax_.
        let y = DenseVector_Double(count: 4,
                                   data: yValuesPtr.baseAddress!)

        SparseMultiplyAdd(alpha, A, x, y)
    }
}

/// On return, `yValues` contains:
///      `[ 281.0, 1.0, 1.0, 401.0 ]`
```

## See Also

### Multiply-Add Functions

func SparseMultiplyAdd(SparseMatrix_Double, DenseVector_Double, DenseVector_Double)

Performs the multiply operation *y += Ax* on a vector of double-precision, floating-point values.

func SparseMultiplyAdd(SparseMatrix_Float, DenseVector_Float, DenseVector_Float)

Performs the multiply operation *y += Ax* on a vector of double-precision, floating-point values.

func SparseMultiplyAdd(Float, SparseMatrix_Float, DenseVector_Float, DenseVector_Float)

Performs the multiply operation *y += alpha \* Ax* on a vector of single-precision, floating-point values.

