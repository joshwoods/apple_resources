

- Metal Performance Shaders
- Matrices and Vectors
-  MPSMatrixFullyConnectedGradient 

Class

# MPSMatrixFullyConnectedGradient

A kernel for applying a fully gradient connected neural network layer.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
class MPSMatrixFullyConnectedGradient : MPSMatrixBinaryKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice)

### Instance Properties

var alpha: Double

var sourceInputFeatureChannels: Int

var sourceNumberOfFeatureVectors: Int

var sourceOutputFeatureChannels: Int

### Instance Methods

func copy(with: NSZone?, device: (any MTLDevice)?) -> Self

func encodeForData(to: any MTLCommandBuffer, gradientMatrix: MPSMatrix, weightMatrix: MPSMatrix, resultGradientForDataMatrix: MPSMatrix)

func encodeForWeightsAndBias(to: any MTLCommandBuffer, gradientMatrix: MPSMatrix, inputMatrix: MPSMatrix, resultGradientForWeightMatrix: MPSMatrix, resultGradientForBiasVector: MPSVector?)

## Relationships

### Inherits From

- MPSMatrixBinaryKernel

## See Also

### Matrix Neural Network Operations

class MPSMatrixFullyConnected

A kernel for applying a fully connected neural network layer.

class MPSMatrixNeuron

A neuron activation kernel that operates on matrices.

class MPSMatrixNeuronGradient

A gradient neuron activation kernel that operates on matrices.

