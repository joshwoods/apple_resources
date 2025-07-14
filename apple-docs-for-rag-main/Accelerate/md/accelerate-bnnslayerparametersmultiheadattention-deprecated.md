

- Accelerate
-  BNNSLayerParametersMultiheadAttention Deprecated

Structure

# BNNSLayerParametersMultiheadAttention

A structure that contains the parameters of a multihead attention layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSLayerParametersMultiheadAttention
```

Deprecated

Use BNNSGraph\* APIs

## Topics

### Initializers

init(query: BNNSMHAProjectionParameters, key: BNNSMHAProjectionParameters, value: BNNSMHAProjectionParameters, add_zero_attn: Bool, key_attn_bias: BNNSNDArrayDescriptor, value_attn_bias: BNNSNDArrayDescriptor, output: BNNSMHAProjectionParameters, dropout: Float, seed: UInt32)

Returns a new multihead attention layer parameters structure from the specified parameters.

init()

Returns a new multihead attention layer parameters structure.

### Instance Properties

var query: BNNSMHAProjectionParameters

A projection parameter structure that describes the query-related input parameters and projection.

var key: BNNSMHAProjectionParameters

A projection parameter structure that describes the key-related input parameters and projection.

var value: BNNSMHAProjectionParameters

A projection parameter structure that describes the value-related input parameters and projection.

var add_zero_attn: Bool

A Boolean value that, if true, adds a row of zeroes to the projected *K* and *V* inputs to the calculation.

var key_attn_bias: BNNSNDArrayDescriptor

A 2D tensor that’s added to the value as part of the attention calculation.

var value_attn_bias: BNNSNDArrayDescriptor

An optional `d_value` x `num_heads` 2D tensor that’s added as part of the attention calculation.

var output: BNNSMHAProjectionParameters

A projection parameter structure that describes the output tensor and associated projection.

var dropout: Float

The seed for the dropout layer’s random number generator.

var seed: UInt32

A random seed for the dropout layer.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Multihead attention layers

struct BNNSMHAProjectionParameters

A structure that contains multihead attention projection parameters.

func BNNSFilterCreateLayerMultiheadAttention(UnsafePointer&lt;BNNSLayerParametersMultiheadAttention>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new multihead attention layer.

Deprecated

func BNNSApplyMultiheadAttention(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeRawPointer, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;Int>?, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;Int>?, UnsafeMutableRawPointer?) -> Int32

Applies a mutihead attention filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSApplyMultiheadAttentionBackward(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSMHAProjectionParameters>?, UnsafeRawPointer?, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeMutablePointer&lt;BNNSMHAProjectionParameters>?, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSMHAProjectionParameters>?, UnsafePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSMHAProjectionParameters>, Int, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;Int>?, UnsafeMutableRawPointer?) -> Int32

Applies a multihead attention filter backward to generate gradients.

Deprecated

