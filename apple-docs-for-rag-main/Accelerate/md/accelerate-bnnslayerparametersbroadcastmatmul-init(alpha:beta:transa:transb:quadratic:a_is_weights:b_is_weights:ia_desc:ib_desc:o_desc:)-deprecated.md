

- Accelerate
- BNNSLayerParametersBroadcastMatMul
-  init(alpha:beta:transA:transB:quadratic:a_is_weights:b_is_weights:iA_desc:iB_desc:o_desc:) Deprecated

Initializer

# init(alpha:beta:transA:transB:quadratic:a_is_weights:b_is_weights:iA_desc:iB_desc:o_desc:)

Returns a new broadcast matrix multiply layer parameters structure from the specified parameters.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    alpha: Float,
    beta: Float,
    transA: Bool,
    transB: Bool,
    quadratic: Bool,
    a_is_weights: Bool,
    b_is_weights: Bool,
    iA_desc: BNNSNDArrayDescriptor,
    iB_desc: BNNSNDArrayDescriptor,
    o_desc: BNNSNDArrayDescriptor
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`alpha`  

A value to scale the result.

`beta`  

A value, that must be either 0.0 or 1.0, you use to scale the existing output before the operation adds it to the result.

`transA`  

A Boolean value that transposes the last two dimensions of matrix *A*.

`transB`  

A Boolean value that transposes the last two dimensions of matrix *B*.

`quadratic`  

A Boolean value that determines whether the operation multiplies matrix *A* by itself.

`a_is_weights`  

A Boolean value that determines whether to treat matrix *A* as weights.

`b_is_weights`  

A Boolean value that determines whether to treat matrix *B* as weights.

`iA_desc`  

The descriptor of matrix *A*.

`iB_desc`  

The descriptor of matrix *B*.

`o_desc`  

The descriptor of the output.

## See Also

### Initializers

init()

Returns a new broadcast matrix multiply layer parameters structure.

Deprecated

