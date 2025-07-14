

- Accelerate
- BNNSLayerParametersMultiheadAttention
-  init(query:key:value:add_zero_attn:key_attn_bias:value_attn_bias:output:dropout:seed:) Deprecated

Initializer

# init(query:key:value:add_zero_attn:key_attn_bias:value_attn_bias:output:dropout:seed:)

Returns a new multihead attention layer parameters structure from the specified parameters.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    query: BNNSMHAProjectionParameters,
    key: BNNSMHAProjectionParameters,
    value: BNNSMHAProjectionParameters,
    add_zero_attn: Bool,
    key_attn_bias: BNNSNDArrayDescriptor,
    value_attn_bias: BNNSNDArrayDescriptor,
    output: BNNSMHAProjectionParameters,
    dropout: Float,
    seed: UInt32
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`query`  

A projection parameter structure that describes the query-related input parameters and projection.

`key`  

A projection parameter structure that describes the key-related input parameters and projection.

`value`  

A projection parameter structure that describes the value-related input parameters and projection.

`add_zero_attn`  

A Boolean value that, if true, adds a row of zeroes to the projected *K* and *V* inputs to the calculation.

`key_attn_bias`  

A 2D tensor that’s added to the key as part of the attention calculation.

`value_attn_bias`  

A 2D tensor that’s added to the value as part of the attention calculation.

`output`  

A projection parameter structure that describes the output tensor and associated projection.

`dropout`  

The probability that the layer drops out an element.

`seed`  

The seed for the dropout layer’s random number generator.

## See Also

### Initializers

init()

Returns a new multihead attention layer parameters structure.

Deprecated

