

- ML Compute
- MLCLSTMResultMode
-  debugDescription 

Instance Property

# debugDescription

A textual description of the LSTM result mode you use for debugging.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+

``` source
var debugDescription: String { get }
```

## See Also

### Enumeration Cases

case output

A result mode that indicates the layer produces a single result tensor that represents the final output of the LSTM.

Deprecated

case outputAndStates

A result mode that indicates the layer produces three result tensors that represent the final output of the LSTM, the last hidden state, and the cell state.

Deprecated

