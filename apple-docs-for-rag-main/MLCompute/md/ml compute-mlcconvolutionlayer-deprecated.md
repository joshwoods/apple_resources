

- ML Compute
-  MLCConvolutionLayer Deprecated

Class

# MLCConvolutionLayer

A layer that applies a convolution over a signal.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCConvolutionLayer
```

## Topics

### Creating Convolution Layers

convenience init?(weights: MLCTensor, biases: MLCTensor?, descriptor: MLCConvolutionDescriptor)

Creates a convolution layer with the weights, biases, and descriptor you specify.

class MLCConvolutionDescriptor

A configuration object you use to create a convolution or fully connected layer.

### Inspecting Convolution Layers

var descriptor: MLCConvolutionDescriptor

The configuration object you use to create the convolution layer.

var weights: MLCTensor

The weights tensor you use for the convolution layer.

var biases: MLCTensor?

The biases tensor you use for the convolution layer.

var weightsParameter: MLCTensorParameter

The weights tensor parameter you use for optimizer updates.

var biasesParameter: MLCTensorParameter?

The biases tensor parameter you use for optimizer updates.

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

### Convolution and Recurrent Layers

class MLCLSTMLayer

A layer that represents long short-term memory (LSTM) networks.

Deprecated

class MLCPoolingLayer

A layer that summarizes the average presence of a feature.

Deprecated

class MLCUpsampleLayer

A layer that applies upsampling with the shape you specify.

Deprecated

class MLCEmbeddingLayer

A layer that stores a word embedding.

Deprecated

