

- Metal Performance Shaders
- Convolutional Neural Network Kernels
-  MPSCNNArithmeticGradient 

Class

# MPSCNNArithmeticGradient

The base class for gradient arithmetic operators.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.0+macOS 10.13.4+tvOS 11.3+visionOS 1.0+

``` source
class MPSCNNArithmeticGradient : MPSCNNGradientKernel
```

## Topics

### Instance Properties

var bias: Float

var isSecondarySourceFilter: Bool

var maximumValue: Float

var minimumValue: Float

var primaryScale: Float

var secondaryScale: Float

var secondaryStrideInFeatureChannels: Int

## Relationships

### Inherits From

- MPSCNNGradientKernel

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

class MPSCNNArithmetic

The base class for arithmetic operators.

class MPSCNNArithmeticGradientState

An object that stores the clamp mask used by gradient arithmetic operators.

