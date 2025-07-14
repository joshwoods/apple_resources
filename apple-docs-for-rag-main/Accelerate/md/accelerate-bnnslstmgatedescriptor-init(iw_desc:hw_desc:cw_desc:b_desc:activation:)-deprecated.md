

- Accelerate
- BNNSLSTMGateDescriptor
-  init(iw_desc:hw_desc:cw_desc:b_desc:activation:) Deprecated

Initializer

# init(iw_desc:hw_desc:cw_desc:b_desc:activation:)

Returns a new long short-term memory (LSTM) gate descriptor structure from the specified parameters.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    iw_desc: (BNNSNDArrayDescriptor, BNNSNDArrayDescriptor),
    hw_desc: BNNSNDArrayDescriptor,
    cw_desc: BNNSNDArrayDescriptor,
    b_desc: BNNSNDArrayDescriptor,
    activation: BNNSActivation
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`iw_desc`  

The descriptor of the input weights.

`hw_desc`  

The descriptor of the hidden weights.

`cw_desc`  

The descriptor of the cell weights.

`b_desc`  

The descriptor of the bias.

`activation`  

The activation function that the layer applies to the output.

## See Also

### Initializers

init()

Returns a new long short-term memory (LSTM) gate descriptor structure.

Deprecated

