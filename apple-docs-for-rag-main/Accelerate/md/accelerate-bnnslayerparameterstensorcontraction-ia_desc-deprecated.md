

- Accelerate
- BNNSLayerParametersTensorContraction
-  iA_desc Deprecated

Instance Property

# iA_desc

The descriptor of input matrix *A*.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
var iA_desc: BNNSNDArrayDescriptor
```

Deprecated

Use BNNSGraph\* APIs

## See Also

### Instance Properties

var operation: UnsafePointer&lt;CChar>

The string that describes the operation.

Deprecated

var alpha: Float

Scaling that the operation applies to the result.

Deprecated

var beta: Float

A value, that must be either 0.0 or 1.0, you use to scale the existing output before the operation adds it to the result.

Deprecated

var iB_desc: BNNSNDArrayDescriptor

The descriptor of input matrix *B*.

Deprecated

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

Deprecated

