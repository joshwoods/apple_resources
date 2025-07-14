

- ML Compute
- MLCActivationDescriptor
-  init(type:a:) Deprecated

Initializer

# init(type:a:)

Creates an activation descriptor with the activation type and parameter a that you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init?(
    type activationType: MLCActivationType,
    a: Float
)
```

## Parameters 

`activationType`  

A type of activation function.

`a`  

Parameter a.

## Discussion

Use this initializer to create one of the following activation descriptors:

CELU  
`f(x) = max(0, x) + min(0, a * (exp(x / a) − 1))`

Activation type: MLCActivationType.celu

For common behavior, set `a` to `1.0`.

HardShrink  
`f(x) = x`, if `x > a` or `x MLCActivationType.hardShrink

For common behavior, set `a` to `0.5`.

Parametric ELU  
`f(x) = x >= 0 ? x : a * (exp(x) - 1)`

Activation type: MLCActivationType.elu

For common behavior, set `a` to `1.0`.

ReLU  
`f(x) = x >= 0 ? x : a * x`

Activation type: MLCActivationType.relu

This is also referred to as Leaky ReLU. Some literature defines classical ReLU as `max(0, x)`. If you want this common behavior, set `a` to `0.0`.

SoftShrink  
`f(x) = x - a`, if `x > a, x + a`, if `x MLCActivationType.softShrink

For common behavior, set `a` to `0.5`.

## See Also

### Creating Activation Descriptors

convenience init?(type: MLCActivationType)

Creates an activation descriptor with the activation type you specify.

Deprecated

convenience init?(type: MLCActivationType, a: Float, b: Float)

Creates an activation descriptor with the activation type and parameters a and b that you specify.

Deprecated

convenience init?(type: MLCActivationType, a: Float, b: Float, c: Float)

Creates an activation descriptor with the activation type and parameters a, b, and c that you specify.

Deprecated

enum MLCActivationType

An activation type that you specify for an activation descriptor.

Deprecated

