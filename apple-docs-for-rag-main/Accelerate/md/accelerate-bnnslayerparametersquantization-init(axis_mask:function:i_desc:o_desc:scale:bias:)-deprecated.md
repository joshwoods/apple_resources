

- Accelerate
- BNNSLayerParametersQuantization
-  init(axis_mask:function:i_desc:o_desc:scale:bias:) Deprecated

Initializer

# init(axis_mask:function:i_desc:o_desc:scale:bias:)

Returns a new quantization layer parameters structure using the supplied parameters.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedtvOS 15.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 8.0–11.0Deprecated

``` source
init(
    axis_mask: Int,
    function: BNNSQuantizerFunction,
    i_desc: BNNSNDArrayDescriptor,
    o_desc: BNNSNDArrayDescriptor,
    scale: BNNSNDArrayDescriptor,
    bias: BNNSNDArrayDescriptor
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`axis_mask`  

A bitmask that defines the axis to which the function applies scale and bias. Set to `0` to apply scale and bias to the entire tensor.

`function`  

The quantize function.

`i_desc`  

The descriptor of the input.

`o_desc`  

The descriptor of the output.

`scale`  

The descriptor of the scale.

`bias`  

The descriptor of the bias.

## See Also

### Initializers

init()

Returns a new quantization layer parameters structure.

Deprecated

