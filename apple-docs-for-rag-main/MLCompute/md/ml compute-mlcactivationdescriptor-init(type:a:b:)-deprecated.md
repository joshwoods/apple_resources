

- ML Compute
- MLCActivationDescriptor
-  init(type:a:b:) Deprecated

Initializer

# init(type:a:b:)

Creates an activation descriptor with the activation type and parameters a and b that you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init?(
    type activationType: MLCActivationType,
    a: Float,
    b: Float
)
```

## Parameters 

`activationType`  

A type of activation function.

`a`  

Parameter a.

`b`  

Parameter b.

## Discussion

Use this initializer to create one of the following activation descriptors:

Hard Sigmoid  
`f(x) = clamp((x * a) + b, 0, 1)`

Activation type: MLCActivationType.hardSigmoid

For common behavior, set `a` to `0.2` and `b` to `0.5`.

Hyperbolic tangent (TanH)  
`f(x) = a * tanh(b * x)`

Activation type: MLCActivationType.tanh

For common behavior, set `a` to `1.0` and `b` to `1.0`.

Linear  
`f(x) = a * x + b`

Activation type: MLCActivationType.linear

For common behavior, set `a` to `1.0` and `b` to `0.0`.

Parametric Soft Plus  
`f(x) = a * log(1 + e^(b * x))`

Activation type: MLCActivationType.softPlus

For common behavior, set `a` to `1.0` and `b` to `1.0`.

ReLUN  
`f(x) = min((x >= 0 ? x : a * x), b)`

Activation type: MLCActivationType.relun

For common behavior, set `a` to `0.0` and `b` to `6.0`.

Threshold  
`f(x) = x`, if `x > a`, else `b`, where:

`a = threshold`

`b = replacement`

Activation type: MLCActivationType.threshold

## See Also

### Creating Activation Descriptors

convenience init?(type: MLCActivationType)

Creates an activation descriptor with the activation type you specify.

Deprecated

convenience init?(type: MLCActivationType, a: Float)

Creates an activation descriptor with the activation type and parameter a that you specify.

Deprecated

convenience init?(type: MLCActivationType, a: Float, b: Float, c: Float)

Creates an activation descriptor with the activation type and parameters a, b, and c that you specify.

Deprecated

enum MLCActivationType

An activation type that you specify for an activation descriptor.

Deprecated

