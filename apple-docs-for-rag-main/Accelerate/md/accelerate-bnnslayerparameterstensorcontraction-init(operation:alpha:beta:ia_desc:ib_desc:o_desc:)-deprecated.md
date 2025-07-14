

- Accelerate
- BNNSLayerParametersTensorContraction
-  init(operation:alpha:beta:iA_desc:iB_desc:o_desc:) Deprecated

Initializer

# init(operation:alpha:beta:iA_desc:iB_desc:o_desc:)

Returns a new tensor-contraction parameters structure.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    operation: UnsafePointer,
    alpha: Float,
    beta: Float,
    iA_desc: BNNSNDArrayDescriptor,
    iB_desc: BNNSNDArrayDescriptor,
    o_desc: BNNSNDArrayDescriptor
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`operation`  

The string that describes the operation.

`alpha`  

Scaling that the operation applies to the result.

`beta`  

A value, that must be either 0.0 or 1.0, you use to scale the existing output before the operation adds it to the result.

`iA_desc`  

The descriptor of input matrix *A*.

`iB_desc`  

The descriptor of input matrix *B*.

`o_desc`  

The descriptor of the output.

