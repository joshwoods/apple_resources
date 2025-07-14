

- ML Compute
- MLCActivationLayer
-  threshold(\_:replacement:) Deprecated

Type Method

# threshold(\_:replacement:)

Creates an instance of a threshold activation layer using the threshold and replacement values you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class func threshold(
    _ threshold: Float,
    replacement: Float
) -> Self
```

## Parameters 

`threshold`  

The threshold value.

`replacement`  

The replacement value.

## Return Value

A new `MLCActivationLayer` instance.

## Discussion

The threshold(_:replacement:) factory type method creates an activation descriptor using init(type:a:b:), where `type =` MLCActivationType.threshold, `a = threshold`, and `b = replacement`, and passes that descriptor to init(descriptor:).

## See Also

### Factory Methods

class func celu(a: Float) -> Self

Creates an instance of a CELU activation layer using the alpha value you specify for the CELU formation.

Deprecated

class func clamp(min: Float, max: Float) -> Self

Creates an instance of a clamp activation layer using the minimum and maximum values you specify for the clamp formation.

Deprecated

class func elu(a: Float) -> Self

Creates an instance of an ELU activation layer using the alpha value you specify for the ELU formation.

Deprecated

class func hardShrink(a: Float) -> Self

Creates an instance of a hard shrink activation layer using the lambda value you specify for the hard shrink formation.

Deprecated

class func leakyReLU(negativeSlope: Float) -> Self

Creates an instance of a leaky ReLU activation layer using the angle of the negative slope you specify.

Deprecated

class func linear(scale: Float, bias: Float) -> Self

Creates an instance of a linear activation layer using the scale factor and bias value you specify.

Deprecated

class func relun(a: Float, b: Float) -> Self

Creates an instance of a ReLUN activation layer using the alpha and beta values you specify.

Deprecated

class func softPlus(beta: Float) -> Self

Creates an instance of a soft plus activation layer using the beta value you specify for the soft plus formation.

Deprecated

class func softShrink(a: Float) -> Self

Creates an instance of a soft shrink activation layer using the lambda value you specify for the soft shrink formation.

Deprecated

