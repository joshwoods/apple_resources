

- Accelerate
- BNNS
- BNNS.FusedNormalizationParameters
-  epsilon Deprecated

Instance Property

# epsilon

The epsilon in the computation of the standard deviation.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+watchOS 8.0+visionOS

``` source
var epsilon: Float
```

Deprecated

Use the BNNSGraph API instead.

## See Also

### Inspecting the Properties of a Fused Normalization Parameters Structure

var type: BNNS.NormalizationType

An enumeration that specifies the normalization type.

Deprecated

var beta: BNNSNDArrayDescriptor?

The descriptor of the beta.

Deprecated

var gamma: BNNSNDArrayDescriptor?

The descriptor of the gamma.

Deprecated

var momentum: Float

A value, between 0 and 1, the normalization operation uses to update the moving mean and moving variance during training.

Deprecated

var activation: BNNS.ActivationFunction

The activation function that the layer applies to the output.

Deprecated

