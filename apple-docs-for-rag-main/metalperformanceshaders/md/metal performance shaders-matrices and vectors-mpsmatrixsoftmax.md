

- Metal Performance Shaders
- Matrices and Vectors
-  MPSMatrixSoftMax 

Class

# MPSMatrixSoftMax

A softmax kernel that operates on matrices.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSMatrixSoftMax : MPSMatrixUnaryKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice)

### Instance Properties

var sourceColumns: Int

var sourceRows: Int

### Instance Methods

func copy(with: NSZone?, device: (any MTLDevice)?) -> Self

func encode(commandBuffer: any MTLCommandBuffer, inputMatrix: MPSMatrix, resultMatrix: MPSMatrix)

## Relationships

### Inherits From

- MPSMatrixUnaryKernel

## See Also

### Matrix Softmax Operations

class MPSMatrixLogSoftMax

A logarithmic softmax kernel that operates on matrices.

class MPSMatrixLogSoftMaxGradient

A logarithmic gradient softmax kernel that operates on matrices.

class MPSMatrixSoftMaxGradient

A gradient softmax kernel that operates on matrices.

