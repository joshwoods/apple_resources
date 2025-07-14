

- Metal Performance Shaders
- Matrices and Vectors
-  MPSMatrixNeuronGradient 

Class

# MPSMatrixNeuronGradient

A gradient neuron activation kernel that operates on matrices.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
class MPSMatrixNeuronGradient : MPSMatrixBinaryKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice)

### Instance Properties

var alpha: Double

var sourceInputFeatureChannels: Int

var sourceNumberOfFeatureVectors: Int

### Instance Methods

func copy(with: NSZone?, device: (any MTLDevice)?) -> Self

func encode(to: any MTLCommandBuffer, gradientMatrix: MPSMatrix, inputMatrix: MPSMatrix, biasVector: MPSVector?, resultGradientForDataMatrix: MPSMatrix, resultGradientForBiasVector: MPSVector?)

func neuronParameterA() -> Float

func neuronParameterB() -> Float

func neuronParameterC() -> Float

func neuronType() -> MPSCNNNeuronType

func setNeuronToPReLUWithParametersA(Data)

func setNeuronType(MPSCNNNeuronType, parameterA: Float, parameterB: Float, parameterC: Float)

## Relationships

### Inherits From

- MPSMatrixBinaryKernel

## See Also

### Matrix Neural Network Operations

class MPSMatrixFullyConnected

A kernel for applying a fully connected neural network layer.

class MPSMatrixFullyConnectedGradient

A kernel for applying a fully gradient connected neural network layer.

class MPSMatrixNeuron

A neuron activation kernel that operates on matrices.

