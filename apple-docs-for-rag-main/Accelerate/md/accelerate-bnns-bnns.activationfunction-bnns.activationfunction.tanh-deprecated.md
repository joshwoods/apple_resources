

- Accelerate
- BNNS
- BNNS.ActivationFunction
-  BNNS.ActivationFunction.tanh Deprecated

Case

# BNNS.ActivationFunction.tanh

An activation function that returns the hyperbolic tangent of its input.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
case tanh
```

Deprecated

Use the BNNSGraph API instead.

## Discussion

This constant defines an activation function that returns values using the following operation:

```
tanh(x)
```

The following illustrates the output that the activation function generates from inputs in the range `-10...10`:

## See Also

### Activation Functions

case abs

An activation function that returns the absolute value of its input.

Deprecated

case celu(alpha: Float)

An activation function that evaluates the continuously differentiable exponential linear units (CELU) on its input.

Deprecated

case clamp(bounds: ClosedRange&lt;Float>)

An activation function that returns its input clamped to the specified range.

Deprecated

case clampedLeakyRectifiedLinear(alpha: Float, beta: Float)

An activation function that returns its input clamped to beta when that is greater than or equal to zero, otherwise it returns its input multiplied by alpha clamped to beta.

Deprecated

case elu(alpha: Float)

An activation function that evaluates the exponential linear units (ELU) on its input.

Deprecated

case geluApproximation(alpha: Float, beta: Float)

An activation function that evaluates the Gaussian error linear units (GELU) approximation on its input.

Deprecated

case geluApproximation2(alpha: Float, beta: Float)

An activation function that provides a fast evaluation of the Gaussian error linear units (GELU) approximation on its input.

Deprecated

case gumbel(alpha: Float, beta: Float)

An activation function that returns random numbers from the Gumbel distribution.

Deprecated

case gumbelMax(alpha: Float, beta: Float)

An activation function that returns random numbers from the Gumbel distribution.

Deprecated

case hardShrink(alpha: Float)

An activation function that returns zero when the absolute input is less than alpha, otherwise it returns its input.

Deprecated

case hardSigmoid(alpha: Float, beta: Float)

An activation function that returns the hard sigmoid function of its input.

Deprecated

case hardSwish(alpha: Float, beta: Float)

An activation function that returns the hard swish function of its input.

Deprecated

case identity

An activation function that returns its input.

Deprecated

case leakyRectifiedLinear(alpha: Float)

An activation function that returns its input when that is greater than or equal to zero, otherwise it returns its input multiplied by a specified value.

Deprecated

case linear(alpha: Float)

An activation function that returns its input multiplied by a specified value.

Deprecated

