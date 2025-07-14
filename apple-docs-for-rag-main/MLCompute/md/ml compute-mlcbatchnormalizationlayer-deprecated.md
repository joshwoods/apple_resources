

- ML Compute
-  MLCBatchNormalizationLayer Deprecated

Class

# MLCBatchNormalizationLayer

A layer that normalizes a batch of inputs.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCBatchNormalizationLayer
```

## Topics

### Creating Batch Normalization Layers

convenience init?(featureChannelCount: Int, mean: MLCTensor, variance: MLCTensor, beta: MLCTensor?, gamma: MLCTensor?, varianceEpsilon: Float)

Creates a batch normalization layer with the number of feature channels, tensors, and variance epsilon you specify.

convenience init?(featureChannelCount: Int, mean: MLCTensor, variance: MLCTensor, beta: MLCTensor?, gamma: MLCTensor?, varianceEpsilon: Float, momentum: Float)

Creates a batch normalization layer with the number of feature channels, tensors, variance epsilon, and momentum you specify.

### Inspecting Batch Normalization Layers

var featureChannelCount: Int

The number of feature channels.

var mean: MLCTensor

The mean tensor.

var variance: MLCTensor

The variance tensor.

var beta: MLCTensor?

The beta tensor.

var gamma: MLCTensor?

The gamma tensor.

var varianceEpsilon: Float

The variance epsilon you use for numerical stability.

var momentum: Float

The value you use for the running mean and variance computation.

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

class MLCGroupNormalizationLayer

A layer that divides the channels into groups for normalization.

Deprecated

class MLCInstanceNormalizationLayer

A layer that normalizes all features of one channel.

Deprecated

class MLCDropoutLayer

A layer that deactivates neurons randomly to avoid overfitting.

Deprecated

