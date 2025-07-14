

- Metal Performance Shaders
- Matrices and Vectors
-  MPSMatrixBatchNormalization 

Class

# MPSMatrixBatchNormalization

A batch normalization kernel that operates on matrices.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
class MPSMatrixBatchNormalization : MPSMatrixUnaryKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice)

### Instance Properties

var computeStatistics: Bool

var epsilon: Float

var sourceInputFeatureChannels: Int

var sourceNumberOfFeatureVectors: Int

### Instance Methods

func copy(with: NSZone?, device: (any MTLDevice)?) -> Self

func encode(commandBuffer: any MTLCommandBuffer, inputMatrix: MPSMatrix, meanVector: MPSVector, varianceVector: MPSVector, gammaVector: MPSVector?, betaVector: MPSVector?, resultMatrix: MPSMatrix)

func neuronParameterA() -> Float

func neuronParameterB() -> Float

func neuronParameterC() -> Float

func neuronType() -> MPSCNNNeuronType

func setNeuronType(MPSCNNNeuronType, parameterA: Float, parameterB: Float, parameterC: Float)

## Relationships

### Inherits From

- MPSMatrixUnaryKernel

## See Also

### Matrix Normalization Operations

class MPSMatrixBatchNormalizationGradient

A batch normalization gradient kernel that operates on matrices.

