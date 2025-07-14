

- ML Compute
-  MLCFullyConnectedLayer Deprecated

Class

# MLCFullyConnectedLayer

A layer that connects each input to each output within its layer.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCFullyConnectedLayer
```

## Overview

This is also known as a dense layer.

## Topics

### Creating Fully Connected Layers

convenience init?(weights: MLCTensor, biases: MLCTensor?, descriptor: MLCConvolutionDescriptor)

Creates a fully connected layer with the weights, biases, and convolution descriptor you specify.

class MLCConvolutionDescriptor

A configuration object you use to create a convolution or fully connected layer.

### Inspecting Fully Connected Layers

var descriptor: MLCConvolutionDescriptor

The configuration object you use to create the fully connected layer.

var weights: MLCTensor

The weights tensor you use for the fully connected layer.

var biases: MLCTensor?

The biases tensor you use for the fully connected layer.

var biasesParameter: MLCTensorParameter?

The biases tensor parameter you use for optimizer updates.

var weightsParameter: MLCTensorParameter

The weights tensor parameter you use for optimizer updates.

## Relationships

### Inherits From

- MLCLayer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Math Layers

class MLCArithmeticLayer

A layer that performs an arithmetic operation.

Deprecated

class MLCReductionLayer

A layer that reduces tensor values across a specific dimension to a scalar value.

Deprecated

class MLCMatMulLayer

A layer that multiplies matrices.

Deprecated

class MLCGramMatrixLayer

A layer that computes the uncentered cross-correlation values between the spacial planes of each feature channel of a tensor.

Deprecated

class MLCComparisonLayer

A layer that performs elementwise comparison of two tensors.

Deprecated

