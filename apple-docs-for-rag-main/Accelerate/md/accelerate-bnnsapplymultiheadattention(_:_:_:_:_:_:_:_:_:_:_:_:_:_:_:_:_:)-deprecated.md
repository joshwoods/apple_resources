

- Accelerate
-  BNNSApplyMultiheadAttention(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSApplyMultiheadAttention(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Applies a mutihead attention filter to a set of input objects, writing the result to a set of output objects.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSApplyMultiheadAttention(
    _ F: BNNSFilter?,
    _ batch_size: Int,
    _ query: UnsafeRawPointer,
    _ query_stride: Int,
    _ key: UnsafeRawPointer,
    _ key_stride: Int,
    _ key_mask: UnsafePointer?,
    _ key_mask_stride: Int,
    _ value: UnsafeRawPointer,
    _ value_stride: Int,
    _ output: UnsafeMutableRawPointer,
    _ output_stride: Int,
    _ add_to_attention: UnsafePointer?,
    _ backprop_cache_size: UnsafeMutablePointer?,
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

Pointer to the data for query input matrix.

`query_stride`  

Batch stride for query.

`key`  

Pointer to the data for key input matrix.

`key_stride`  

Batch stride for key.

`key_mask`  

Mask applied to key for ignoring entries.

`key_mask_stride`  

Batch stride for key mask.

`value`  

Pointer to the data for value input matrix.

`value_stride`  

Batch stride for value.

`output`  

Pointer to the data for output matrix

`output_stride`  

Batch stride for output.

`add_to_attention`  

Pointer to the 2D tensor that’s used as part of the mask function prior to softmax in the attention calculation.

`backprop_cache_size`  

The size of the back propagation cache, in bytes.

`backprop_cache`  

A cache that stores intermediate results that BNNS can use to accelerate a future call to this function.

`workspace_size`  

The size of the array workspace, in bytes.

`workspace`  

A scratch buffer used during the calculation.

## Discussion

Provide `key_mask` as a 1D tensor containing `source_length` elements. Where the elements evaluate to true, the attention operation ignores the corresponding elements of the key matrix.

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

func BNNSApplyMultiheadAttentionBackward(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSMHAProjectionParameters>?, UnsafeRawPointer?, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeMutablePointer&lt;BNNSMHAProjectionParameters>?, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSMHAProjectionParameters>?, UnsafePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSMHAProjectionParameters>, Int, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;Int>?, UnsafeMutableRawPointer?) -> Int32

Applies a multihead attention filter backward to generate gradients.

Deprecated

