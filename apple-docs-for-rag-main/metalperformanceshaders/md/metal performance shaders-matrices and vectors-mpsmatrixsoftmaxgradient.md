

- Metal Performance Shaders
- Matrices and Vectors
-  MPSMatrixSoftMaxGradient 

Class

# MPSMatrixSoftMaxGradient

A gradient softmax kernel that operates on matrices.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
class MPSMatrixSoftMaxGradient : MPSMatrixBinaryKernel
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

func encode(to: any MTLCommandBuffer, gradientMatrix: MPSMatrix, forwardOutputMatrix: MPSMatrix, resultMatrix: MPSMatrix)

## Relationships

### Inherits From

- MPSMatrixBinaryKernel

## See Also

### Matrix Softmax Operations

class MPSMatrixLogSoftMax

A logarithmic softmax kernel that operates on matrices.

class MPSMatrixLogSoftMaxGradient

A logarithmic gradient softmax kernel that operates on matrices.

class MPSMatrixSoftMax

A softmax kernel that operates on matrices.

