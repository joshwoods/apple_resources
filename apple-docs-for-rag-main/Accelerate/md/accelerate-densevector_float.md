

- Accelerate
-  DenseVector_Float 

Structure

# DenseVector_Float

A structure that contains a dense vector of single-precision, floating-point values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct DenseVector_Float
```

## Overview

You typically use dense vectors to represent the unknowns vector, *x*, and the right-hand-side vector, *b*, in the matrix equation *Ax = b.* A DenseVector_Float structure provides a pointer to its underlying data and a count of its number of elements.

The following code shows an example of how to create a dense vector structure from an array of single-precision values. In this case, use withUnsafeMutableBufferPointer(_:) to pass a pointer to your collection. The DenseVector_Float structure is valid only during the execution of the closure. Don’t store or return the structure for later use.

```
var vectorValues: [Float] = [10, 20, 30, 40]
let vectorValuesCount = Int32(vectorValues.count)

vectorValues.withUnsafeMutableBufferPointer { vectorValuesPtr in

    let vector = DenseVector_Float(count: vectorValuesCount,
                                   data: vectorValuesPtr.baseAddress!)

    // Perform operations using `vector`.
}
```

## Topics

### Initializers

init(count: Int32, data: UnsafeMutablePointer&lt;Float>)

Creates a new vector of single-precision values.

### Inspecting a Vector’s Structure and Data

var count: Int32

The number of items in the vector.

var data: UnsafeMutablePointer&lt;Float>

The array of single-precision, floating-point values.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Creating dense matrices and dense vectors

struct DenseMatrix_Double

A structure that contains a dense matrix of double-precision, floating-point values.

struct DenseMatrix_Float

A structure that contains a dense matrix of single-precision, floating-point values.

struct DenseVector_Double

A structure that contains a dense vector of double-precision, floating-point values.

