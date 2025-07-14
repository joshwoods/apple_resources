

- Metal Performance Shaders
- Matrices and Vectors
-  MPSMatrixNeuron 

Class

# MPSMatrixNeuron

A neuron activation kernel that operates on matrices.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSMatrixNeuron : MPSMatrixUnaryKernel
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

func encode(commandBuffer: any MTLCommandBuffer, inputMatrix: MPSMatrix, biasVector: MPSVector?, resultMatrix: MPSMatrix)

func neuronParameterA() -> Float

func neuronParameterB() -> Float

func neuronParameterC() -> Float

func neuronType() -> MPSCNNNeuronType

func setNeuronToPReLUWithParametersA(Data)

func setNeuronType(MPSCNNNeuronType, parameterA: Float, parameterB: Float, parameterC: Float)

## Relationships

### Inherits From

- MPSMatrixUnaryKernel

## See Also

### Matrix Neural Network Operations

class MPSMatrixFullyConnected

A kernel for applying a fully connected neural network layer.

class MPSMatrixFullyConnectedGradient

A kernel for applying a fully gradient connected neural network layer.

class MPSMatrixNeuronGradient

A gradient neuron activation kernel that operates on matrices.

