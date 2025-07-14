

- Metal Performance Shaders
- Matrices and Vectors
-  MPSMatrixSum 

Class

# MPSMatrixSum

A kernel for performing a pointwise summation of a matrix.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSMatrixSum : MPSKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice, count: Int, rows: Int, columns: Int, transpose: Bool)

### Instance Properties

var columns: Int

var count: Int

var neuronParameterA: Float

var neuronParameterB: Float

var neuronParameterC: Float

var resultMatrixOrigin: MTLOrigin

var rows: Int

var transpose: Bool

### Instance Methods

func encode(to: any MTLCommandBuffer, sourceMatrices: [MPSMatrix], resultMatrix: MPSMatrix, scale: MPSVector?, offsetVector: MPSVector?, biasVector: MPSVector?, start: Int)

func neuronType() -> MPSCNNNeuronType

func setNeuronType(MPSCNNNeuronType, parameterA: Float, parameterB: Float, parameterC: Float)

## Relationships

### Inherits From

- MPSKernel

## See Also

### Matrix Arithmetic Operations

class MPSMatrixMultiplication

A matrix multiplication kernel.

class MPSMatrixVectorMultiplication

A matrix-vector multiplication kernel

class MPSMatrixFindTopK

A kernel for computing the top-K values and their corresponding indices in a matrix.

