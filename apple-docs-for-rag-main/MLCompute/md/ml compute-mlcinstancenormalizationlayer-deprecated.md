

- ML Compute
-  MLCInstanceNormalizationLayer Deprecated

Class

# MLCInstanceNormalizationLayer

A layer that normalizes all features of one channel.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCInstanceNormalizationLayer
```

## Topics

### Creating Instance Normalization Layers

convenience init?(featureChannelCount: Int, beta: MLCTensor?, gamma: MLCTensor?, varianceEpsilon: Float)

Creates an instance normalization layer with the number of feature channels, beta and gamma tensors, and variance epsilon you specify.

convenience init?(featureChannelCount: Int, beta: MLCTensor?, gamma: MLCTensor?, varianceEpsilon: Float, momentum: Float)

Creates an instance normalization layer with the number of feature channels, beta and gamma tensors, variance epsilon, and momentum you specify.

convenience init?(featureChannelCount: Int, mean: MLCTensor, variance: MLCTensor, beta: MLCTensor?, gamma: MLCTensor?, varianceEpsilon: Float, momentum: Float)

Creates an instance normalization layer with the number of feature channels, mean, variance, beta and gamma tensors, variance epsilon, and momentum you specify.

### Inspecting Instance Normalization Layers

var beta: MLCTensor?

The beta tensor.

var betaParameter: MLCTensorParameter?

The beta tensor parameter you use for optimizer updates.

var featureChannelCount: Int

The number of feature channels.

var gamma: MLCTensor?

The gamma tensor.

var gammaParameter: MLCTensorParameter?

The gamma tensor parameter you use for optimizer updates.

var mean: MLCTensor?

The running mean tensor.

var momentum: Float

The momentum value for the running mean and variance computation.

var variance: MLCTensor?

The running variance tensor.

var varianceEpsilon: Float

The variance epsilon you use for numerical stability.

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

class MLCGroupNormalizationLayer

A layer that divides the channels into groups for normalization.

Deprecated

class MLCDropoutLayer

A layer that deactivates neurons randomly to avoid overfitting.

Deprecated

