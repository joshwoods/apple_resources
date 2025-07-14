

- ML Compute
-  MLCDropoutLayer Deprecated

Class

# MLCDropoutLayer

A layer that deactivates neurons randomly to avoid overfitting.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCDropoutLayer
```

## Topics

### Creating Dropout Layers

convenience init(rate: Float, seed: Int)

Creates a dropout layer with the probability rate and random number generator seed you specify.

### Inspecting a Dropout Layer

var rate: Float

The dropout rate you use for each element.

var seed: Int

The seed you use to generate random numbers.

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

class MLCInstanceNormalizationLayer

A layer that normalizes all features of one channel.

Deprecated

