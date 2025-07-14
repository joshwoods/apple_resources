

- Accelerate
-  BNNSFilterCreateLayerMultiheadAttention(\_:\_:) Deprecated

Function

# BNNSFilterCreateLayerMultiheadAttention(\_:\_:)

Returns a new multihead attention layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSFilterCreateLayerMultiheadAttention(
    _ layer_params: UnsafePointer,
    _ filter_params: UnsafePointer?
) -> BNNSFilter?
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`layer_params`  

Layer parameters.

`filter_params`  

The filter runtime parameters.

## See Also

### Multihead attention layers

struct BNNSMHAProjectionParameters

A structure that contains multihead attention projection parameters.

struct BNNSLayerParametersMultiheadAttention

A structure that contains the parameters of a multihead attention layer.

Deprecated

func BNNSApplyMultiheadAttention(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeRawPointer, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;Int>?, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;Int>?, UnsafeMutableRawPointer?) -> Int32

Applies a mutihead attention filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSApplyMultiheadAttentionBackward(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSMHAProjectionParameters>?, UnsafeRawPointer?, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeMutablePointer&lt;BNNSMHAProjectionParameters>?, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSMHAProjectionParameters>?, UnsafePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSMHAProjectionParameters>, Int, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;Int>?, UnsafeMutableRawPointer?) -> Int32

Applies a multihead attention filter backward to generate gradients.

Deprecated

