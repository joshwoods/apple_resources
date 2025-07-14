

- Accelerate
- BNNS
- BNNS.FusedNormalizationParameters
-  type Deprecated

Instance Property

# type

An enumeration that specifies the normalization type.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
var type: BNNS.NormalizationType
```

Deprecated

Use the BNNSGraph API instead.

## See Also

### Inspecting the Properties of a Fused Normalization Parameters Structure

var beta: BNNSNDArrayDescriptor?

The descriptor of the beta.

Deprecated

var gamma: BNNSNDArrayDescriptor?

The descriptor of the gamma.

Deprecated

var momentum: Float

A value, between 0 and 1, the normalization operation uses to update the moving mean and moving variance during training.

Deprecated

var epsilon: Float

The epsilon in the computation of the standard deviation.

Deprecated

var activation: BNNS.ActivationFunction

The activation function that the layer applies to the output.

Deprecated

