

- ML Compute
- MLCActivationType
-  MLCActivationType.selu Deprecated

Case

# MLCActivationType.selu

An activation type that implements the scaled exponential linear unit activation function.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
case selu
```

## Discussion

This activation type implements the following function:

`f(x) = scale * (max(0, x) + min(0, α * (exp(x)−1)))`, where:

`α = 1.6732632423543772848170429916717`

`scale = 1.0507009873554804934193349852946`

## See Also

### Enumeration Cases

case absolute

An activation type that implements the absolute activation function.

Deprecated

case celu

An activation type that implements the CELU activation function.

Deprecated

case clamp

An activation type that implements the clamp activation function.

Deprecated

case elu

An activation type that implements the exponential linear unit activation function.

Deprecated

case gelu

An activation type that implements the gaussian error linear unit activation function.

Deprecated

case hardShrink

An activation type that implements the hard shrink activation function.

Deprecated

case hardSigmoid

An activation type that implements the hard sigmoid activation function.

Deprecated

case hardSwish

An activation type that implements the hard swish activation function.

Deprecated

case linear

An activation type that implements the linear activation function.

Deprecated

case logSigmoid

An activation type that implements the log sigmoid activation function.

Deprecated

case none

An activation type that implements the identity function.

Deprecated

case relu

An activation type that implements the rectified linear unit activation function.

Deprecated

case relun

An activation type that implements the ReLUN activation function.

Deprecated

case sigmoid

An activation type that implements the sigmoid activation function.

Deprecated

case softPlus

An activation type that implements the soft plus activation function.

Deprecated

