

- Accelerate
- BNNSLayerParametersBroadcastMatMul
-  a_is_weights Deprecated

Instance Property

# a_is_weights

A Boolean value that determines whether to treat matrix *A* as weights.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
var a_is_weights: Bool
```

Deprecated

Use BNNSGraph\* APIs

## See Also

### Instance Properties

var alpha: Float

A value to scale the result.

Deprecated

var beta: Float

A value, that must be either 0.0 or 1.0, you use to scale the existing output before the operation adds it to the result.

Deprecated

var transA: Bool

A Boolean value that transposes the last two dimensions of matrix *A*.

Deprecated

var transB: Bool

A Boolean value that transposes the last two dimensions of matrix *B*.

Deprecated

var quadratic: Bool

A Boolean value that determines whether the operation multiplies matrix *A* by itself.

Deprecated

var b_is_weights: Bool

A Boolean value that determines whether to treat matrix *B* as weights.

Deprecated

var iA_desc: BNNSNDArrayDescriptor

The descriptor of matrix *A*.

Deprecated

var iB_desc: BNNSNDArrayDescriptor

The descriptor of matrix *B*.

Deprecated

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

Deprecated

