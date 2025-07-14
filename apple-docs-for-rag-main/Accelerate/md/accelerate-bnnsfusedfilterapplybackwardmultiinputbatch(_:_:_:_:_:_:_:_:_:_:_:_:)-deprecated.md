

- Accelerate
-  BNNSFusedFilterApplyBackwardMultiInputBatch(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSFusedFilterApplyBackwardMultiInputBatch(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Applies a multiple-input fused filter backward to generate input gradients.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedtvOS 15.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 8.0–11.0Deprecated

``` source
func BNNSFusedFilterApplyBackwardMultiInputBatch(
    _ filter: BNNSFilter?,
    _ batch_size: Int,
    _ number_of_inputs: Int,
    _ in: UnsafeMutablePointer?,
    _ in_stride: UnsafePointer?,
    _ in_delta: UnsafeMutablePointer>,
    _ in_delta_stride: UnsafePointer,
    _ out: UnsafeRawPointer?,
    _ out_stride: Int,
    _ out_delta: UnsafeMutablePointer,
    _ out_delta_stride: Int,
    _ delta_parameters: UnsafeMutablePointer?>?
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`filter`  

The filter to apply.

`batch_size`  

The number of input-output pairs.

`number_of_inputs`  

The number of inputs for the multiple-input filter.

`in`  

A pointer to the input data.

`in_stride`  

The increment, in values, between inputs.

`in_delta`  

The descriptor of the input delta.

`in_delta_stride`  

The increment, in values, between input delta objects.

`out`  

A pointer to the output data.

`out_stride`  

The increment, in values, between outputs.

`out_delta`  

The descriptor of the input delta.

`out_delta_stride`  

The increment, in values, between output delta objects.

`delta_parameters`  

A pointer to an array of parameter delta pointers.

## See Also

### Fused layers

protocol FusableLayerParametersDeprecated

class FusedParametersLayer

A layer object that wraps a fused layer and manages its deinitialization.

Deprecated

class FusedConvolutionNormalizationLayer

A layer object that wraps a fused, convolution normalization layer and manages its deinitialization.

Deprecated

class FusedFullyConnectedNormalizationLayer

A layer object that wraps a fused, fully connected normalization layer and manages its deinitialization.

Deprecated

struct BNNSFilterType

Constants that define the component filters of a fused layer.

func BNNSFilterCreateFusedLayer(Int, UnsafePointer&lt;BNNSFilterType>, UnsafeMutablePointer&lt;UnsafeRawPointer>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new fused layer.

Deprecated

func BNNSFusedFilterApplyBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, Bool) -> Int32

Applies a fused filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSFusedFilterApplyMultiInputBatch(BNNSFilter?, Int, Int, UnsafeMutablePointer&lt;UnsafeRawPointer>, UnsafePointer&lt;Int>, UnsafeMutableRawPointer, Int, Bool) -> Int32

Applies a multiple-input fused filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSFusedFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?>?) -> Int32

Applies a fused filter backward to generate input gradients.

Deprecated

