

- Metal Performance Shaders
- Convolutional Neural Network Kernels
-  MPSCNNMultiplyGradient 

Class

# MPSCNNMultiplyGradient

A gradient multiply operator.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.0+macOS 10.13.4+tvOS 11.3+visionOS 1.0+

``` source
class MPSCNNMultiplyGradient : MPSCNNArithmeticGradient
```

## Topics

### Initializers

init(device: any MTLDevice, isSecondarySourceFilter: Bool)

## Relationships

### Inherits From

- MPSCNNArithmeticGradient

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

class MPSCNNDivide

A division operator.

class MPSCNNArithmetic

The base class for arithmetic operators.

class MPSCNNArithmeticGradient

The base class for gradient arithmetic operators.

class MPSCNNArithmeticGradientState

An object that stores the clamp mask used by gradient arithmetic operators.

