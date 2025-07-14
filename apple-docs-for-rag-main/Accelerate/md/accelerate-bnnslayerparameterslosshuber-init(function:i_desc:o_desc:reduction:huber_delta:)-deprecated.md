

- Accelerate
- BNNSLayerParametersLossHuber
-  init(function:i_desc:o_desc:reduction:huber_delta:) Deprecated

Initializer

# init(function:i_desc:o_desc:reduction:huber_delta:)

Returns a new Huber loss layer parameters structure from the specified parameters.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    function: BNNSLossFunction,
    i_desc: BNNSNDArrayDescriptor,
    o_desc: BNNSNDArrayDescriptor,
    reduction: BNNSLossReductionFunction,
    huber_delta: Float
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`function`  

The function that’s used to compute loss.

`i_desc`  

The descriptor of the input.

`o_desc`  

The descriptor of the output.

`reduction`  

The function that’s used to reduce the computed loss.

`huber_delta`  

The boundary value that defines where Huber loss returns mean absolute error or mean square error.

## Discussion

Important

The input data type and output data type must be `float`. The output size must be `1`, unless the reduction is BNNS.LossReduction.none.

## See Also

### Initializers

init()

Returns a new Huber loss layer parameters structure.

Deprecated

