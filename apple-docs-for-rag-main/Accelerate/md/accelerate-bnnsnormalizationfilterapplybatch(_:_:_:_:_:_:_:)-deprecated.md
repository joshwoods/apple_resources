

- Accelerate
-  BNNSNormalizationFilterApplyBatch(\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSNormalizationFilterApplyBatch(\_:\_:\_:\_:\_:\_:\_:)

Applies a normalization filter to a set of input objects, writing the result to a set of output objects.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSNormalizationFilterApplyBatch(
    _ filter: BNNSFilter?,
    _ batch_size: Int,
    _ in: UnsafeRawPointer,
    _ in_stride: Int,
    _ out: UnsafeMutableRawPointer,
    _ out_stride: Int,
    _ training: Bool
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`filter`  

The filter to apply.

`batch_size`  

The number of input-output pairs.

`in`  

Pointer to the input data.

`in_stride`  

Increment, in values, between inputs.

`out`  

Pointer to the output data.

`out_stride`  

Increment, in values, between outputs.

`training`  

Set to true during training and false during inference.

## See Also

### Normalization layers

class NormalizationLayer

A layer object that wraps a normalization filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersNormalization

A structure that contains the parameters of a normalization layer.

Deprecated

func BNNSFilterCreateLayerNormalization(BNNSFilterType, UnsafePointer&lt;BNNSLayerParametersNormalization>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new normalization layer.

Deprecated

func BNNSNormalizationFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?) -> Int32

Applies a normalization filter backward to generate gradients.

Deprecated

