

- Accelerate
-  SparseConvertFromOpaque(\_:) 

Function

# SparseConvertFromOpaque(\_:)

Returns a sparse matrix of single-precision, floating-point values from a BLAS opaque matrix.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SparseConvertFromOpaque(_ matrix: sparse_matrix_float) -> SparseMatrix_Float
```

## Parameters 

`matrix`  

The opaque matrix to convert.

## Return Value

A new SparseMatrix_Float.

## Discussion

The following code shows an example of creating a SparseMatrix_Double structure from a BLAS opaque matrix and multiplying it by a vector:

```
guard let blasMatrix = sparse_matrix_create_float(4, 4) else {
    return
}

sparse_insert_entry_float(blasMatrix, 1.0, 0, 0)
sparse_insert_entry_float(blasMatrix, 4.0, 3, 0)
sparse_insert_entry_float(blasMatrix, 13.0, 0, 3)
sparse_insert_entry_float(blasMatrix, 16.0, 3, 3)

let A: SparseMatrix_Float = SparseConvertFromOpaque(blasMatrix)

defer {
    SparseCleanup(A)
}

/// The values for _x_ in _y=Ax_.
var xValues: [Float] = [10.0, -1.0, -1.0, 10.0]

/// The values for _y_ in _y=Ax_.
let yValues = [Float](unsafeUninitializedCapacity: xValues.count) {
    resultBuffer, count in

    xValues.withUnsafeMutableBufferPointer { xValuesPtr in
        /// The _x_ in _y=Ax_.
        let x = DenseVector_Float(count: 4,
                                  data: xValuesPtr.baseAddress!)

        /// The _y_ in _y=Ax_.
        let y = DenseVector_Float(count: 4,
                                  data: resultBuffer.baseAddress!)

        SparseMultiply(A, x, y)
    }

    count = xValues.count
}
```

On return, `yValues` contains the values `[140.0, 0.0, 0.0, 200.0]`.

## See Also

### BLAS Support

func SparseConvertFromOpaque(sparse_matrix_double) -> SparseMatrix_Double

Returns a sparse matrix of double-precision, floating-point values from a BLAS opaque matrix.

