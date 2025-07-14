

- Accelerate
-  BNNSActivationFunctionGumbel 

Global Variable

# BNNSActivationFunctionGumbel

An activation function that returns random numbers from the Gumbel distribution.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var BNNSActivationFunctionGumbel: BNNSActivationFunction { get }
```

## Discussion

This constant defines an activation function that returns values using the following operation:

```
−log(−log(alpha*Uniform(0,1)+beta)+beta)
```

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

var BNNSActivationFunctionGumbelMax: BNNSActivationFunction

An activation function that returns random numbers from the Gumbel distribution.

var BNNSActivationFunctionHardShrink: BNNSActivationFunction

An activation function that returns zero when the absolute input is less than alpha, otherwise it returns its input.

var BNNSActivationFunctionHardSigmoid: BNNSActivationFunction

An activation function that returns the hard sigmoid function of its input.

