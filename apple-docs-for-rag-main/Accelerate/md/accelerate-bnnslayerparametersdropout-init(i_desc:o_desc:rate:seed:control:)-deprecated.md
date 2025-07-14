

- Accelerate
- BNNSLayerParametersDropout
-  init(i_desc:o_desc:rate:seed:control:) Deprecated

Initializer

# init(i_desc:o_desc:rate:seed:control:)

Returns a new dropout layer parameters structure from the specified parameters.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    i_desc: BNNSNDArrayDescriptor,
    o_desc: BNNSNDArrayDescriptor,
    rate: Float,
    seed: UInt32,
    control: UInt8
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`i_desc`  

The descriptor of the input.

`o_desc`  

The descriptor of the output.

`rate`  

The probability that the layer drops out an element or a group of elements.

`seed`  

The seed for the random number generator that the layer ignores if zero.

`control`  

An 8-bit bit mask that indicates the dimension of the grouping of the dropout decision.

## Discussion

Important

Dropout layers only support arrays with a data type of `float`. The input shape must be equal to the output shape.

## See Also

### Initializers

init()

Returns a new dropout layer parameters structure.

Deprecated

