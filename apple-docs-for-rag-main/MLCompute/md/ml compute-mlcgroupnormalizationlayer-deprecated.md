

- ML Compute
-  MLCGroupNormalizationLayer Deprecated

Class

# MLCGroupNormalizationLayer

A layer that divides the channels into groups for normalization.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCGroupNormalizationLayer
```

## Topics

### Creating Group Normalization Layers

convenience init?(featureChannelCount: Int, groupCount: Int, beta: MLCTensor?, gamma: MLCTensor?, varianceEpsilon: Float)

Creates a group normalization layer with the number of feature channels and groups, beta and gamma tensors, and variance epsilon you specify.

### Inspecting Group Normalization Layers

var featureChannelCount: Int

The number of feature channels.

var groupCount: Int

The number of groups into which you separate the channels.

var beta: MLCTensor?

The beta tensor.

var gamma: MLCTensor?

The gamma tensor.

var varianceEpsilon: Float

The variance epsilon you use for numerical stability.

var betaParameter: MLCTensorParameter?

The beta tensor parameter you use for optimizer updates.

var gammaParameter: MLCTensorParameter?

The gamma tensor parameter you use for optimizer updates.

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

### Normalization Layers

class MLCLayerNormalizationLayer

A layer that applies layer normalization over inputs.

Deprecated

class MLCBatchNormalizationLayer

A layer that normalizes a batch of inputs.

Deprecated

class MLCInstanceNormalizationLayer

A layer that normalizes all features of one channel.

Deprecated

class MLCDropoutLayer

A layer that deactivates neurons randomly to avoid overfitting.

Deprecated

