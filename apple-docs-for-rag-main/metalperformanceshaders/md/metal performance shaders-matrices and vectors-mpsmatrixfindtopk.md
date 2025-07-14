

- Metal Performance Shaders
- Matrices and Vectors
-  MPSMatrixFindTopK 

Class

# MPSMatrixFindTopK

A kernel for computing the top-K values and their corresponding indices in a matrix.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.0+macOS 10.13.4+tvOS 11.3+visionOS 1.0+

``` source
class MPSMatrixFindTopK : MPSMatrixUnaryKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice, numberOfTopKValues: Int)

### Instance Properties

var indexOffset: Int

var numberOfTopKValues: Int

var sourceColumns: Int

var sourceRows: Int

### Instance Methods

func copy(with: NSZone?, device: (any MTLDevice)?) -> Self

func encode(commandBuffer: any MTLCommandBuffer, inputMatrix: MPSMatrix, resultIndexMatrix: MPSMatrix, resultValueMatrix: MPSMatrix)

## Relationships

### Inherits From

- MPSMatrixUnaryKernel

## See Also

### Matrix Arithmetic Operations

class MPSMatrixSum

A kernel for performing a pointwise summation of a matrix.

class MPSMatrixMultiplication

A matrix multiplication kernel.

class MPSMatrixVectorMultiplication

A matrix-vector multiplication kernel

