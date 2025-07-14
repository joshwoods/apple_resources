

- Accelerate
- BNNSLayerParametersQuantization
-  axis_mask Deprecated

Instance Property

# axis_mask

A bitmask that defines the axis to which the function applies scale and bias.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedtvOS 15.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 8.0–11.0Deprecated

``` source
var axis_mask: Int
```

Deprecated

Use BNNSGraph\* APIs

## Discussion

Set to `0` to apply scale and bias to the entire tensor.

## See Also

### Instance Properties

var function: BNNSQuantizerFunction

The quantize function.

Deprecated

var i_desc: BNNSNDArrayDescriptor

The descriptor of the input.

Deprecated

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

Deprecated

var scale: BNNSNDArrayDescriptor

The descriptor of the scale.

Deprecated

var bias: BNNSNDArrayDescriptor

The descriptor of the bias.

Deprecated

