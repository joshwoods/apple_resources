

- Accelerate
- BNNS
- BNNS.ActivationFunction
-  BNNS.ActivationFunction.softmax Deprecated

Case

# BNNS.ActivationFunction.softmax

An activation function that returns the softmax function of its input.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
case softmax
```

Deprecated

Use the BNNSGraph API instead.

## Discussion

This constant defines an activation function that returns values using the following formula:

The softmax function transforms a vector of real numbers into a vector of probabilities. Each probability in the result is in the range 0…1, and the sum of the probabilities is 1.

For example, given and array that contains the values `[3.0, 5.0, 1.0, 6.0, 2.0, 1.0, 4.0]`, the softmax function calculates the following values:

| Inputs | Outputs       |
|--------|---------------|
| `3.0`  | `0.031415492` |
| `5.0`  | `0.23213086`  |
| `1.0`  | `0.004251625` |
| `6.0`  | `0.63099706`  |
| `2.0`  | `0.011557114` |
| `1.0`  | `0.004251625` |
| `4.0`  | `0.08539616`  |

Changing the fourth element from `6.0` to `10.0` increases its probability to almost 1.0:

| Inputs | Outputs         |
|--------|-----------------|
| `3.0`  | `0.00090221845` |
| `5.0`  | `0.0066665425`  |
| `1.0`  | `0.00012210199` |
| `10.0` | `0.98940265`    |
| `2.0`  | `0.00033190762` |
| `1.0`  | `0.00012210199` |
| `4.0`  | `0.002452484`   |

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

