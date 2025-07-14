

- Accelerate
- BNNSLSTMDataDescriptor
-  init(data_desc:hidden_desc:cell_state_desc:) Deprecated

Initializer

# init(data_desc:hidden_desc:cell_state_desc:)

Returns a new long short-term memory (LSTM) data descriptor structure from the specified parameters.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    data_desc: BNNSNDArrayDescriptor,
    hidden_desc: BNNSNDArrayDescriptor,
    cell_state_desc: BNNSNDArrayDescriptor
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`data_desc`  

The descriptor of the input-output.

`hidden_desc`  

The descriptor of the hidden input-output.

`cell_state_desc`  

The descriptor of the cell-state input-output.

## See Also

### Initializers

init()

Returns a new long short-term memory (LSTM) data descriptor structure.

Deprecated

