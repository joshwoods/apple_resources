

- Accelerate
-  BNNSActivationFunctionLeakyRectifiedLinear 

Global Variable

# BNNSActivationFunctionLeakyRectifiedLinear

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+visionOSwatchOS 3.0+tvOS 10.0+

``` source
var BNNSActivationFunctionLeakyRectifiedLinear: BNNSActivationFunction
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

var BNNSActivationFunctionGumbel: BNNSActivationFunction

An activation function that returns random numbers from the Gumbel distribution.

var BNNSActivationFunctionGumbelMax: BNNSActivationFunction

An activation function that returns random numbers from the Gumbel distribution.

var BNNSActivationFunctionHardShrink: BNNSActivationFunction

An activation function that returns zero when the absolute input is less than alpha, otherwise it returns its input.

