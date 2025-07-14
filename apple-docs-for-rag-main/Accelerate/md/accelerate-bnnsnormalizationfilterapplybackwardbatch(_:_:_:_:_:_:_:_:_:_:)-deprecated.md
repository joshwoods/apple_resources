

- Accelerate
-  BNNSNormalizationFilterApplyBackwardBatch(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSNormalizationFilterApplyBackwardBatch(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Applies a normalization filter backward to generate gradients.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSNormalizationFilterApplyBackwardBatch(
    _ filter: BNNSFilter?,
    _ batch_size: Int,
    _ in_delta: UnsafeMutablePointer?,
    _ in_delta_stride: Int,
    _ out: UnsafeRawPointer?,
    _ out_stride: Int,
    _ out_delta: UnsafeMutablePointer,
    _ out_delta_stride: Int,
    _ beta_delta: UnsafeMutablePointer?,
    _ gamma_delta: UnsafeMutablePointer?
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`filter`  

The filter to apply.

`batch_size`  

The number of input-output pairs.

`in_delta`  

The descriptor of the input delta.

`in_delta_stride`  

Increment, in values, between input delta objects.

`out`  

Pointer to output object.

`out_stride`  

Increment, in values, between output objects.

`out_delta`  

The descriptor of the output delta.

`out_delta_stride`  

Increment, in values, between output delta objects.

`beta_delta`  

The descriptor of the beta delta.

`gamma_delta`  

The descriptor of the gamma delta.

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

func BNNSNormalizationFilterApplyBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, Bool) -> Int32

Applies a normalization filter to a set of input objects, writing the result to a set of output objects.

Deprecated

