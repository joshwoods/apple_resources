

- Accelerate
-  DenseVector_Double 

Structure

# DenseVector_Double

A structure that contains a dense vector of double-precision, floating-point values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct DenseVector_Double
```

## Mentioned in 

Solving systems using iterative methods

Solving systems using direct methods

## Overview

You typically use dense vectors to represent the unknowns vector, *x*, and the right-hand-side vector, *b*, in the matrix equation *Ax = b.* A DenseVector_Double structure provides a pointer to its underlying data and a count of its number of elements.

The following code shows an example of how to create a dense vector structure from an array of double-precision values. In this case, use withUnsafeMutableBufferPointer(_:) to pass a pointer to your collection. The DenseVector_Double structure is valid only during the execution of the closure. Don’t store or return the structure for later use.

```
var vectorValues: [Double] = [10, 20, 30, 40]
let vectorValuesCount = Int32(vectorValues.count)

vectorValues.withUnsafeMutableBufferPointer { vectorValuesPtr in

    let vector = DenseVector_Double(count: vectorValuesCount,
                                    data: vectorValuesPtr.baseAddress!)

    // Perform operations using `vector`.
}
```

## Topics

### Initializers

init(count: Int32, data: UnsafeMutablePointer&lt;Double>)

Creates a new vector of double-precision values.

### Inspecting a Vector’s Structure and Data

var count: Int32

The number of items in the vector.

var data: UnsafeMutablePointer&lt;Double>

The array of double-precision, floating-point values.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Creating dense matrices and dense vectors

struct DenseMatrix_Double

A structure that contains a dense matrix of double-precision, floating-point values.

struct DenseMatrix_Float

A structure that contains a dense matrix of single-precision, floating-point values.

struct DenseVector_Float

A structure that contains a dense vector of single-precision, floating-point values.

