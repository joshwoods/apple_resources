

- Metal Performance Shaders
- Matrices and Vectors
-  MPSMatrixVectorMultiplication 

Class

# MPSMatrixVectorMultiplication

A matrix-vector multiplication kernel

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSMatrixVectorMultiplication : MPSMatrixBinaryKernel
```

## Topics

### Initializers

init(device: any MTLDevice, transpose: Bool, rows: Int, columns: Int, alpha: Double, beta: Double)

init(device: any MTLDevice, rows: Int, columns: Int)

### Instance Methods

func encode(commandBuffer: any MTLCommandBuffer, inputMatrix: MPSMatrix, inputVector: MPSVector, resultVector: MPSVector)

## Relationships

### Inherits From

- MPSMatrixBinaryKernel

## See Also

### Matrix Arithmetic Operations

class MPSMatrixSum

A kernel for performing a pointwise summation of a matrix.

class MPSMatrixMultiplication

A matrix multiplication kernel.

class MPSMatrixFindTopK

A kernel for computing the top-K values and their corresponding indices in a matrix.

