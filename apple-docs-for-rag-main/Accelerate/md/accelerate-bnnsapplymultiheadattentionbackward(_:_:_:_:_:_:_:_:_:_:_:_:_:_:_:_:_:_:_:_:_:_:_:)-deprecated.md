

- Accelerate
-  BNNSApplyMultiheadAttentionBackward(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSApplyMultiheadAttentionBackward(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Applies a multihead attention filter backward to generate gradients.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSApplyMultiheadAttentionBackward(
    _ F: BNNSFilter?,
    _ batch_size: Int,
    _ query: UnsafeRawPointer?,
    _ query_stride: Int,
    _ query_param_delta: UnsafeMutablePointer?,
    _ key: UnsafeRawPointer?,
    _ key_stride: Int,
    _ key_mask: UnsafePointer?,
    _ key_mask_stride: Int,
    _ key_param_delta: UnsafeMutablePointer?,
    _ value: UnsafeRawPointer?,
    _ value_stride: Int,
    _ value_param_delta: UnsafeMutablePointer?,
    _ add_to_attention: UnsafePointer?,
    _ key_attn_bias_delta: UnsafeMutablePointer?,
    _ value_attn_bias_delta: UnsafeMutablePointer?,
    _ output: UnsafeRawPointer?,
    _ output_stride: Int,
    _ output_param_delta: UnsafeMutablePointer,
    _ backprop_cache_size: Int,
    _ backprop_cache: UnsafeMutableRawPointer?,
    _ workspace_size: UnsafeMutablePointer?,
    _ workspace: UnsafeMutableRawPointer?
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`F`  

The filter to apply.

`batch_size`  

The number of input-output pairs.

`query`  

Pointer to data for query input matrix.

`query_stride`  

Batch stride for query.

`query_param_delta`  

Pointer to the data structure used to hold deltas for corresponding components.

`key`  

Pointer to data for key input matrix.

`key_stride`  

Batch stride for key.

`key_mask`  

Mask applied to key for ignoring entries.

`key_mask_stride`  

Batch stride for key mask.

`key_param_delta`  

Pointer to the data structure used to hold deltas for corresponding components.

`value`  

Pointer to the data for value input matrix,.

`value_stride`  

Batch stride for value.

`value_param_delta`  

Pointer to the data structure used to hold deltas for corresponding components.

`add_to_attention`  

Pointer to the 2D tensor that’s used as part of the mask function prior to softmax in the attention calculation.

`key_attn_bias_delta`  

Pointer to the data structure used to hold deltas for corresponding components.

`value_attn_bias_delta`  

Pointer to the data structure used to hold deltas for corresponding components.

`output`  

Pointer to the data for output matrix.

`output_stride`  

Batch stride for output.

`output_param_delta`  

Pointer to the data structure used to hold deltas for corresponding components.

`backprop_cache_size`  

The size of the back propagation cache, in bytes.

`backprop_cache`  

A cache that stores intermediate results that BNNS can use to accelerate a future call to this function.

`workspace_size`  

The size of the array workspace, in bytes.

`workspace`  

A scratch buffer used during the calculation.

## See Also

### Multihead attention layers

struct BNNSMHAProjectionParameters

A structure that contains multihead attention projection parameters.

struct BNNSLayerParametersMultiheadAttention

A structure that contains the parameters of a multihead attention layer.

Deprecated

func BNNSFilterCreateLayerMultiheadAttention(UnsafePointer&lt;BNNSLayerParametersMultiheadAttention>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new multihead attention layer.

Deprecated

func BNNSApplyMultiheadAttention(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeRawPointer, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;Int>?, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;Int>?, UnsafeMutableRawPointer?) -> Int32

Applies a mutihead attention filter to a set of input objects, writing the result to a set of output objects.

Deprecated

