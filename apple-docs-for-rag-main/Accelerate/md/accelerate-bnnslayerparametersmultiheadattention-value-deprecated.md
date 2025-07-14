

- Accelerate
- BNNSLayerParametersMultiheadAttention
-  value Deprecated

Instance Property

# value

A projection parameter structure that describes the value-related input parameters and projection.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
var value: BNNSMHAProjectionParameters
```

Deprecated

Use BNNSGraph\* APIs

## See Also

### Instance Properties

var query: BNNSMHAProjectionParameters

A projection parameter structure that describes the query-related input parameters and projection.

Deprecated

var key: BNNSMHAProjectionParameters

A projection parameter structure that describes the key-related input parameters and projection.

Deprecated

var add_zero_attn: Bool

A Boolean value that, if true, adds a row of zeroes to the projected *K* and *V* inputs to the calculation.

Deprecated

var key_attn_bias: BNNSNDArrayDescriptor

A 2D tensor that’s added to the value as part of the attention calculation.

Deprecated

var value_attn_bias: BNNSNDArrayDescriptor

An optional `d_value` x `num_heads` 2D tensor that’s added as part of the attention calculation.

Deprecated

var output: BNNSMHAProjectionParameters

A projection parameter structure that describes the output tensor and associated projection.

Deprecated

var dropout: Float

The seed for the dropout layer’s random number generator.

Deprecated

var seed: UInt32

A random seed for the dropout layer.

Deprecated

