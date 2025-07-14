

- Accelerate
-  BNNSPermuteFilterApplyBackwardBatch(\_:\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSPermuteFilterApplyBackwardBatch(\_:\_:\_:\_:\_:\_:)

Applies a permute filter backward to generate gradients.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSPermuteFilterApplyBackwardBatch(
    _ filter: BNNSFilter?,
    _ batch_size: Int,
    _ in_delta: UnsafeMutablePointer,
    _ in_delta_stride: Int,
    _ out_delta: UnsafePointer,
    _ out_delta_stride: Int
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`filter`  

The filter to apply.

`batch_size`  

Number of input-output pairs to process.

`in_delta`  

The descriptor of the input delta.

`in_delta_stride`  

Increment, in values, between input delta objects.

`out_delta`  

The descriptor of the output delta.

`out_delta_stride`  

Increment, in values, between output delta objects.

## See Also

### Permute layers

class PermuteLayer

A layer object that wraps a permute filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersPermute

A structure that contains the parameters of a permute layer.

Deprecated

func BNNSFilterCreateLayerPermute(UnsafePointer&lt;BNNSLayerParametersPermute>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new permute layer.

Deprecated

