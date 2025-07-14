

- ML Compute
-  MLCEmbeddingLayer Deprecated

Class

# MLCEmbeddingLayer

A layer that stores a word embedding.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCEmbeddingLayer
```

## Topics

### Creating Embedding Layers

convenience init(descriptor: MLCEmbeddingDescriptor, weights: MLCTensor)

Creates an embedding layer with the descriptor and word embedding weights tensor you specify.

class MLCEmbeddingDescriptor

A configuration object you use to create an embedding layer.

### Inspecting Embedding Layers

var descriptor: MLCEmbeddingDescriptor

The configuration object you use to create the embedding layer.

var weights: MLCTensor

The weights tensor that contains the word embedding.

var weightsParameter: MLCTensorParameter

The tensor parameter that describes the weights for the optimizer update.

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

class MLCConvolutionLayer

A layer that applies a convolution over a signal.

Deprecated

class MLCLSTMLayer

A layer that represents long short-term memory (LSTM) networks.

Deprecated

class MLCPoolingLayer

A layer that summarizes the average presence of a feature.

Deprecated

class MLCUpsampleLayer

A layer that applies upsampling with the shape you specify.

Deprecated

