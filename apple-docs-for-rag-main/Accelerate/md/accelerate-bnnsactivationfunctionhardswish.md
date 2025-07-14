

- Accelerate
-  BNNSActivationFunctionHardSwish 

Global Variable

# BNNSActivationFunctionHardSwish

An activation function that returns the hard swish function of its input.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var BNNSActivationFunctionHardSwish: BNNSActivationFunction { get }
```

## Discussion

This constant defines an activation function that returns values using the following operation:

```
HardSwish(x) = x * (ReLU6(x + 3.0) * 1.0/6.0)
```

The following illustrates the output that the activation function generates from inputs in the range `-10...10`:

## See Also

### Raw Values

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

var BNNSActivationFunctionAbs: BNNSActivationFunctionDeprecated

var BNNSActivationFunctionCELU: BNNSActivationFunction

An activation function that evaluates the continuously differentiable exponential linear units (CELU) on its input.

var BNNSActivationFunctionClampedLeakyRectifiedLinear: BNNSActivationFunction

An activation function that returns its input clamped to beta when that is greater than or equal to zero, otherwise it returns its input multiplied by alpha clamped to beta.

var BNNSActivationFunctionELU: BNNSActivationFunction

An activation function that evaluates the exponential linear units (ELU) on its input.

var BNNSActivationFunctionErf: BNNSActivationFunction

var BNNSActivationFunctionGELU: BNNSActivationFunction

var BNNSActivationFunctionGELUApproximation: BNNSActivationFunction

An activation function that evaluates the Gaussian error linear units (GELU) approximation on its input.

var BNNSActivationFunctionGELUApproximation2: BNNSActivationFunction

An activation function that provides a fast evaluation of the Gaussian error linear units (GELU) approximation on its input.

var BNNSActivationFunctionGELUApproximationSigmoid: BNNSActivationFunction

var BNNSActivationFunctionGumbel: BNNSActivationFunction

An activation function that returns random numbers from the Gumbel distribution.

var BNNSActivationFunctionGumbelMax: BNNSActivationFunction

An activation function that returns random numbers from the Gumbel distribution.

var BNNSActivationFunctionHardShrink: BNNSActivationFunction

An activation function that returns zero when the absolute input is less than alpha, otherwise it returns its input.

