

- ML Compute
-  MLCUpsampleLayer Deprecated

Class

# MLCUpsampleLayer

A layer that applies upsampling with the shape you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCUpsampleLayer
```

## Topics

### Creating Upsample Layers

convenience init?(shape: [Int])

Creates an upsample layer with the shape you specify.

convenience init?(shape: [Int], sampleMode: MLCSampleMode, alignsCorners: Bool)

Creates an upsample layer with the shape, upsampling algorithm, and corner alignment option you specify.

enum MLCSampleMode

A sampling mode for an upsample layer.

### Inspecting Upsample Layers

var shape: [Int]

An array that contains the dimensions of the result tensor.

var sampleMode: MLCSampleMode

The upsampling algorithm type.

var alignsCorners: Bool

A Boolean that indicates whether the layer aligns the corner pixels of the input and output tensors.

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

class MLCEmbeddingLayer

A layer that stores a word embedding.

Deprecated

