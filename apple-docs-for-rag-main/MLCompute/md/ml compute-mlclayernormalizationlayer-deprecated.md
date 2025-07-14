

- ML Compute
-  MLCLayerNormalizationLayer Deprecated

Class

# MLCLayerNormalizationLayer

A layer that applies layer normalization over inputs.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCLayerNormalizationLayer
```

## Topics

### Creating Layer Normalization Layers

convenience init?(normalizedShape: [Int], beta: MLCTensor, gamma: MLCTensor, varianceEpsilon: Float)

Creates a normalization layer with a shape, beta and gamma tensors, and variance epsilon you specify.

convenience init?(normalizedShape: [Int], beta: MLCTensor?, gamma: MLCTensor?, varianceEpsilon: Float)

Creates a normalization layer with a shape, optional beta and gamma tensors, and variance epsilon you specify.

### Inspecting Layer Normalization Layers

var normalizedShape: [Int]

The shape of the axes where normalization occurs.

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

class MLCBatchNormalizationLayer

A layer that normalizes a batch of inputs.

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

