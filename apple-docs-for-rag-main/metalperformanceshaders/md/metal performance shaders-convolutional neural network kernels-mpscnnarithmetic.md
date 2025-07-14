

- Metal Performance Shaders
- Convolutional Neural Network Kernels
-  MPSCNNArithmetic 

Class

# MPSCNNArithmetic

The base class for arithmetic operators.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.0+macOS 10.13.4+tvOS 11.3+visionOS 1.0+

``` source
class MPSCNNArithmetic : MPSCNNBinaryKernel
```

## Topics

### Instance Properties

var bias: Float

var maximumValue: Float

var minimumValue: Float

var primaryScale: Float

var primaryStrideInFeatureChannels: Int

var secondaryScale: Float

var secondaryStrideInFeatureChannels: Int

### Instance Methods

func encode(commandBuffer: any MTLCommandBuffer, primaryImage: MPSImage, secondaryImage: MPSImage, destinationState: MPSCNNArithmeticGradientState, destinationImage: MPSImage)

func encodeBatch(commandBuffer: any MTLCommandBuffer, primaryImages: [MPSImage], secondaryImages: [MPSImage], destinationStates: [MPSCNNArithmeticGradientState], destinationImages: [MPSImage])

## Relationships

### Inherits From

- MPSCNNBinaryKernel

## See Also

### Arithmetic Layers

class MPSCNNAdd

An addition operator.

class MPSCNNAddGradient

A gradient addition operator.

class MPSCNNSubtract

A subtraction operator.

class MPSCNNSubtractGradient

A gradient subtraction operator.

class MPSCNNMultiply

A multiply operator.

class MPSCNNMultiplyGradient

A gradient multiply operator.

class MPSCNNDivide

A division operator.

class MPSCNNArithmeticGradient

The base class for gradient arithmetic operators.

class MPSCNNArithmeticGradientState

An object that stores the clamp mask used by gradient arithmetic operators.

