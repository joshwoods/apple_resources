

- Accelerate
- BNNSLayerParametersNormalization
-  moving_variance_desc Deprecated

Instance Property

# moving_variance_desc

The descriptor of the moving variance.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
var moving_variance_desc: BNNSNDArrayDescriptor
```

Deprecated

Use BNNSGraph\* APIs

## See Also

### Instance Properties

var i_desc: BNNSNDArrayDescriptor

The descriptor of the input.

Deprecated

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

Deprecated

var beta_desc: BNNSNDArrayDescriptor

The descriptor of the beta or bias.

Deprecated

var gamma_desc: BNNSNDArrayDescriptor

The descriptor of the gamma or scale.

Deprecated

var moving_mean_desc: BNNSNDArrayDescriptor

The descriptor of the moving mean.

Deprecated

var momentum: Float

A value, between 0 and 1, the normalization operation uses to update the moving mean and moving variance during training.

Deprecated

var epsilon: Float

The epsilon in the computation of the standard deviation.

Deprecated

var activation: BNNSActivation

The activation function that the layer applies to the output.

Deprecated

var num_groups: Int

The number of groups over which the layer computes normalization statistics.

Deprecated

var normalization_axis: Int

The axis on which a layer normalization operation starts normalization.

Deprecated

