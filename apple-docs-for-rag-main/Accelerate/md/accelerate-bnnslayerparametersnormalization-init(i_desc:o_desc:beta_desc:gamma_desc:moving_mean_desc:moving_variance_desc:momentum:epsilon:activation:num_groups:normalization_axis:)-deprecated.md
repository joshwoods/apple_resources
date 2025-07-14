

- Accelerate
- BNNSLayerParametersNormalization
-  init(i_desc:o_desc:beta_desc:gamma_desc:moving_mean_desc:moving_variance_desc:momentum:epsilon:activation:num_groups:normalization_axis:) Deprecated

Initializer

# init(i_desc:o_desc:beta_desc:gamma_desc:moving_mean_desc:moving_variance_desc:momentum:epsilon:activation:num_groups:normalization_axis:)

Returns a new normalization layer parameters structure from the specified parameters.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    i_desc: BNNSNDArrayDescriptor,
    o_desc: BNNSNDArrayDescriptor,
    beta_desc: BNNSNDArrayDescriptor,
    gamma_desc: BNNSNDArrayDescriptor,
    moving_mean_desc: BNNSNDArrayDescriptor,
    moving_variance_desc: BNNSNDArrayDescriptor,
    momentum: Float,
    epsilon: Float,
    activation: BNNSActivation,
    num_groups: Int,
    normalization_axis: Int
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`i_desc`  

The descriptor of the input.

`o_desc`  

The descriptor of the output.

`beta_desc`  

The descriptor of the beta or bias.

`gamma_desc`  

The descriptor of the gamma or scale.

`moving_mean_desc`  

The descriptor of the moving mean.

`moving_variance_desc`  

The descriptor of the moving variance.

`momentum`  

A value, between 0 and 1, the normalization operation uses to update the moving mean and moving variance during training.

`epsilon`  

The epsilon in the computation of the standard deviation.

`activation`  

The activation function that the layer applies to the output.

`num_groups`  

The number of groups over which the layer computes normalization statistics.

`normalization_axis`  

The axis on which a layer normalization operation starts normalization.

## Discussion

moving_mean_desc and moving_variance_desc are only applicable to batch- and instance-normalization.

Important

The gamma and beta descriptors must match the shape of input up to the normalizaton axis. The input and output descriptors must have a layout of BNNS.DataLayout.imageCHW. The gamma, beta, moving mean, and moving variance descriptors must have a `size[0]` that’s the same as the number of input channels. All arrays must have a data type of `float`.

## See Also

### Initializers

init()

Returns a new normalization layer parameters structure.

Deprecated

