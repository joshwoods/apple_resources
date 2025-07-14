

- Accelerate
- BNNSLayerParametersPadding
-  init(i_desc:o_desc:padding_size:padding_mode:padding_value:) Deprecated

Initializer

# init(i_desc:o_desc:padding_size:padding_mode:padding_value:)

Returns a new padding-layer parameters structure from the specified parameters.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    i_desc: BNNSNDArrayDescriptor,
    o_desc: BNNSNDArrayDescriptor,
    padding_size: ((Int, Int), (Int, Int), (Int, Int), (Int, Int), (Int, Int), (Int, Int), (Int, Int), (Int, Int)),
    padding_mode: BNNSPaddingMode,
    padding_value: UInt32
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`i_desc`  

The descriptor of the input.

`o_desc`  

The descriptor of the output.

`padding_size`  

The number of padding elements to add before and after the original data.

`padding_mode`  

The mode the operation uses to pad.

`padding_value`  

The value the operation uses to fill the padding area when the mode is constant.

## Discussion

Important

Padding isn’t supported beyond 4D tensors.

## See Also

### Initializers

init()

Returns a new padding-layer parameters structure.

Deprecated

