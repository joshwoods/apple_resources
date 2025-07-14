

- Accelerate
-  BNNSLayerParametersNormalization Deprecated

Structure

# BNNSLayerParametersNormalization

A structure that contains the parameters of a normalization layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSLayerParametersNormalization
```

Deprecated

Use BNNSGraph\* APIs

## Topics

### Initializers

init(i_desc: BNNSNDArrayDescriptor, o_desc: BNNSNDArrayDescriptor, beta_desc: BNNSNDArrayDescriptor, gamma_desc: BNNSNDArrayDescriptor, moving_mean_desc: BNNSNDArrayDescriptor, moving_variance_desc: BNNSNDArrayDescriptor, momentum: Float, epsilon: Float, activation: BNNSActivation, num_groups: Int, normalization_axis: Int)

Returns a new normalization layer parameters structure from the specified parameters.

init()

Returns a new normalization layer parameters structure.

### Instance Properties

var i_desc: BNNSNDArrayDescriptor

The descriptor of the input.

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

var beta_desc: BNNSNDArrayDescriptor

The descriptor of the beta or bias.

var gamma_desc: BNNSNDArrayDescriptor

The descriptor of the gamma or scale.

var moving_mean_desc: BNNSNDArrayDescriptor

The descriptor of the moving mean.

var moving_variance_desc: BNNSNDArrayDescriptor

The descriptor of the moving variance.

var momentum: Float

A value, between 0 and 1, the normalization operation uses to update the moving mean and moving variance during training.

var epsilon: Float

The epsilon in the computation of the standard deviation.

var activation: BNNSActivation

The activation function that the layer applies to the output.

var num_groups: Int

The number of groups over which the layer computes normalization statistics.

var normalization_axis: Int

The axis on which a layer normalization operation starts normalization.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Normalization layers

class NormalizationLayer

A layer object that wraps a normalization filter and manages its deinitialization.

Deprecated

func BNNSFilterCreateLayerNormalization(BNNSFilterType, UnsafePointer&lt;BNNSLayerParametersNormalization>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new normalization layer.

Deprecated

func BNNSNormalizationFilterApplyBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, Bool) -> Int32

Applies a normalization filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSNormalizationFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?) -> Int32

Applies a normalization filter backward to generate gradients.

Deprecated

