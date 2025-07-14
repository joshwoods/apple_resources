

- Accelerate
- BNNSLayerParametersFullyConnected
-  init(i_desc:w_desc:o_desc:bias:activation:) Deprecated

Initializer

# init(i_desc:w_desc:o_desc:bias:activation:)

Returns a new fully connected layer parameters structure from the specified parameters.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    i_desc: BNNSNDArrayDescriptor,
    w_desc: BNNSNDArrayDescriptor,
    o_desc: BNNSNDArrayDescriptor,
    bias: BNNSNDArrayDescriptor,
    activation: BNNSActivation
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`i_desc`  

The descriptor of the input.

`w_desc`  

The descriptor of the weights.

`o_desc`  

The descriptor of the output.

`bias`  

The descriptor of the bias.

`activation`  

The activation function that the layer applies to the output.

## Discussion

Important

The input data type and the weights data type must be equal and be `float`, `float16`, `int8`, or `int16` for the forward pass. The output data type must be `float` for the forward pass. All three arrays must be `float` for the backward pass.

## See Also

### Initializers

init()

Returns a new fully connected layer parameters structure.

Deprecated

