

- ML Compute
-  MLCPoolingLayer Deprecated

Class

# MLCPoolingLayer

A layer that summarizes the average presence of a feature.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCPoolingLayer
```

## Topics

### Creating Pooling Layers

convenience init(descriptor: MLCPoolingDescriptor)

Creates a pooling layer with the descriptor you specify.

class MLCPoolingDescriptor

A configuration object you use to create a pooling layer.

enum MLCPoolingType

A pooling function type for a pooling layer.

### Inspecting Pooling Layers

var descriptor: MLCPoolingDescriptor

The configuration object you use to create the pooling layer.

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

class MLCUpsampleLayer

A layer that applies upsampling with the shape you specify.

Deprecated

class MLCEmbeddingLayer

A layer that stores a word embedding.

Deprecated

