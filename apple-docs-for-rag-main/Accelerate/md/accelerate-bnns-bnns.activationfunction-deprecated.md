

- Accelerate
- BNNS
-  BNNS.ActivationFunction Deprecated

Enumeration

# BNNS.ActivationFunction

Constants that describe activation functions.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
enum ActivationFunction
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Activation Functions

case abs

An activation function that returns the absolute value of its input.

case celu(alpha: Float)

An activation function that evaluates the continuously differentiable exponential linear units (CELU) on its input.

case clamp(bounds: ClosedRange&lt;Float>)

An activation function that returns its input clamped to the specified range.

case clampedLeakyRectifiedLinear(alpha: Float, beta: Float)

An activation function that returns its input clamped to beta when that is greater than or equal to zero, otherwise it returns its input multiplied by alpha clamped to beta.

case elu(alpha: Float)

An activation function that evaluates the exponential linear units (ELU) on its input.

case geluApproximation(alpha: Float, beta: Float)

An activation function that evaluates the Gaussian error linear units (GELU) approximation on its input.

case geluApproximation2(alpha: Float, beta: Float)

An activation function that provides a fast evaluation of the Gaussian error linear units (GELU) approximation on its input.

case gumbel(alpha: Float, beta: Float)

An activation function that returns random numbers from the Gumbel distribution.

case gumbelMax(alpha: Float, beta: Float)

An activation function that returns random numbers from the Gumbel distribution.

case hardShrink(alpha: Float)

An activation function that returns zero when the absolute input is less than alpha, otherwise it returns its input.

case hardSigmoid(alpha: Float, beta: Float)

An activation function that returns the hard sigmoid function of its input.

case hardSwish(alpha: Float, beta: Float)

An activation function that returns the hard swish function of its input.

case identity

An activation function that returns its input.

case leakyRectifiedLinear(alpha: Float)

An activation function that returns its input when that is greater than or equal to zero, otherwise it returns its input multiplied by a specified value.

case linear(alpha: Float)

An activation function that returns its input multiplied by a specified value.

case linearWithBias(alpha: Float, beta: Float)

An activation function that returns its input multiplied by a scale and added to a bias.

case logSigmoid

An activation function that returns the logarithm of the sigmoid function of its input.

case logSoftmax

An activation function that returns the logarithm of the softmax function of its input.

case rectifiedLinear

An activation function that returns its input when that is greater than or equal to zero, otherwise it returns zero.

case scaledTanh(alpha: Float, beta: Float)

An activation function that returns the scaled hyperbolic tangent of its input.

case selu

An activation function that evaluates the scaled exponential linear units (SELU) on its input.

case sigmoid

An activation function that returns the sigmoid function of its input.

case silu

An activation function that returns the sigmoid linear unit (SiLU) function of its input.

case softShrink(alpha: Float)

An activation function that returns zero when the absolute input is less than alpha, otherwise it returns its input minus alpha.

case softmax

An activation function that returns the softmax function of its input.

case softplus(alpha: Float, beta: Float)

An activation function that returns the softplus function of its input.

case softsign

An activation function that returns the softsign function of its input.

case tanh

An activation function that returns the hyperbolic tangent of its input.

case tanhShrink

An activation function that returns its input minus the hyperbolic tangent of its input.

case threshold(alpha: Float, beta: Float)

An activation function that returns beta if its input is less than a specified threshold, otherwise it returns its input.

### Instance Properties

var bnnsActivation: BNNSActivation

The underlying activation function.

