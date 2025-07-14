

- Accelerate
-  DenseMatrix_Float 

Structure

# DenseMatrix_Float

A structure that contains a dense matrix of single-precision, floating-point values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct DenseMatrix_Float
```

## Overview

You typically use dense matrices to represent the unknowns matrix, *X*, and the right-hand-side matrix, *B*, in the matrix equation *AX = B.* A DenseMatrix_Float structure provides a pointer to its underlying data, and information about its structure and attributes.

The following code shows an example of how to create a dense matrix structure from an array of double-precision values. In this case, use withUnsafeMutableBufferPointer(_:) to pass a pointer to your collection. The DenseMatrix_Float structure is valid only during the execution of the closure. Don’t store or return the structure for later use.

```
// An array of `rowCount` x `columnCount` single-precision values.
var matrixValues = [...]
let rowCount = Int32(5)
let columnCount = Int32(5)

matrixValues.withUnsafeMutableBufferPointer {
    let matrix = DenseMatrix_Float(rowCount: rowCount,
                                   columnCount: columnCount,
                                   columnStride: rowCount,
                                   attributes: SparseAttributes_t(),
                                   data: $0.baseAddress!)

    // Perform operations using `matrix`.
}
```

## Topics

### Initializers

init(rowCount: Int32, columnCount: Int32, columnStride: Int32, attributes: SparseAttributes_t, data: UnsafeMutablePointer&lt;Float>)

Creates a new matrix of single-precision values.

### Inspecting a Matrix’s Structure and Data

var rowCount: Int32

The number of rows in the matrix.

var columnCount: Int32

The number of columns in the matrix.

var columnStride: Int32

The stride between matrix columns, in elements.

var attributes: SparseAttributes_t

The attributes of the matrix, such as whether it’s symmetrical or triangular.

struct SparseAttributes_t

A structure that represents the attributes of a matrix.

var data: UnsafeMutablePointer&lt;Float>

The array of single-precision, floating-point values in column-major order.

## See Also

### Creating dense matrices and dense vectors

struct DenseMatrix_Double

A structure that contains a dense matrix of double-precision, floating-point values.

struct DenseVector_Double

A structure that contains a dense vector of double-precision, floating-point values.

struct DenseVector_Float

A structure that contains a dense vector of single-precision, floating-point values.

