

- Accelerate
- BNNSLayerParametersActivation
-  init(i_desc:o_desc:activation:axis_flags:) Deprecated

Initializer

# init(i_desc:o_desc:activation:axis_flags:)

Returns a new activation layer parameters structure from the supplied descriptors, activation function, and axis flags.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    i_desc: BNNSNDArrayDescriptor,
    o_desc: BNNSNDArrayDescriptor,
    activation: BNNSActivation,
    axis_flags: UInt32
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`i_desc`  

The descriptor of the input.

`o_desc`  

The descriptor of the output.

`activation`  

The activation function that the layer applies to the output.

`axis_flags`  

Flags that indicate axes on which the layer applies certain activation functions.

## Discussion

Important

The input dimensions must be equal to the output dimensions. For activation types other than identity, the input and output must be `float`.

## See Also

### Initializers

init()

Returns a new activation layer parameters structure.

Deprecated

