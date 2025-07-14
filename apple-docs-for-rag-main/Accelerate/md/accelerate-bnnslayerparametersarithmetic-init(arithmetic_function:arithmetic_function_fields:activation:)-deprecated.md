

- Accelerate
- BNNSLayerParametersArithmetic
-  init(arithmetic_function:arithmetic_function_fields:activation:) Deprecated

Initializer

# init(arithmetic_function:arithmetic_function_fields:activation:)

Returns a new arithmetic layer parameters structure.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    arithmetic_function: BNNSArithmeticFunction,
    arithmetic_function_fields: UnsafeMutableRawPointer,
    activation: BNNSActivation
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`arithmetic_function`  

The arithmetic function.

`arithmetic_function_fields`  

A pointer to an arithmetic function field structure.

`activation`  

The activation function that the layer applies to the output.

