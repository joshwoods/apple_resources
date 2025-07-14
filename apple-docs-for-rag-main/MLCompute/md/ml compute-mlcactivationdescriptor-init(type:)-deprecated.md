

- ML Compute
- MLCActivationDescriptor
-  init(type:) Deprecated

Initializer

# init(type:)

Creates an activation descriptor with the activation type you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init?(type activationType: MLCActivationType)
```

## Parameters 

`activationType`  

A type of activation function.

## Discussion

Use this initializer to create one of the following activation descriptors:

Absolute  
`f(x) = fabs(x)`

Activation type: MLCActivationType.absolute

GELU  
`f(x) = x * CDF(x)`

Activation type: MLCActivationType.gelu

Hard Swish  
`f(x) = 0, if x = +3`

`f(x) = x * (x + 3)/6`

Activation type: MLCActivationType.hardSwish

Identity  
`f(x) = x`

Activation type: MLCActivationType.none

LogSigmoid  
`f(x) = log(1 / (1 + exp(-x)))`

Activation type: MLCActivationType.logSigmoid

Parametric Soft Sign  
`f(x) = x / (1 + abs(x))`

Activation type: MLCActivationType.softSign

SELU  
`f(x) = scale * (max(0, x) + min(0, α * (exp(x)−1)))`, where:

`α = 1.6732632423543772848170429916717`

`scale = 1.0507009873554804934193349852946`

Activation type: MLCActivationType.selu

Sigmoid  
`f(x) = 1 / (1 + e⁻ˣ)`

Activation type: MLCActivationType.sigmoid

TanhShrink  
`f(x) = x - tanh(x)`

Activation type: MLCActivationType.tanhShrink

## See Also

### Creating Activation Descriptors

convenience init?(type: MLCActivationType, a: Float)

Creates an activation descriptor with the activation type and parameter a that you specify.

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

