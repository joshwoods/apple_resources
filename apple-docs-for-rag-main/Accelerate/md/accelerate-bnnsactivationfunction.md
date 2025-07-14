

- Accelerate
-  BNNSActivationFunction 

Structure

# BNNSActivationFunction

Constants that describe activation functions.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSActivationFunction
```

## Topics

### Activation Functions

static var abs: BNNSActivationFunction

An activation function that returns the absolute value of its input.

Deprecated

static var clamp: BNNSActivationFunction

An activation function that returns its input clamped to a specified range.

Deprecated

static var identity: BNNSActivationFunction

An activation function that returns its input.

Deprecated

static var integerLinearSaturate: BNNSActivationFunction

An activation function that returns an arithmetic shift, preserving sign.

Deprecated

static var integerLinearSaturatePerChannel: BNNSActivationFunction

An activation function that returns an arithmetic shift, preserving sign for each channel.

Deprecated

static var leakyRectifiedLinear: BNNSActivationFunction

An activation function that returns its input when that is greater than or equal to zero, otherwise it returns its input multiplied by a specified value.

Deprecated

static var linear: BNNSActivationFunction

An activation function that returns its input multiplied by a specified value.

Deprecated

static var rectifiedLinear: BNNSActivationFunction

An activation function that returns its input when that is greater than or equal to zero, otherwise it returns zero.

Deprecated

static var scaledTanh: BNNSActivationFunction

An activation function that returns the scaled hyperbolic tangent of its input.

Deprecated

static var sigmoid: BNNSActivationFunction

An activation function that returns the sigmoid function of its input.

Deprecated

static var softmax: BNNSActivationFunction

An activation function that returns the softmax function of its input.

Deprecated

static var tanh: BNNSActivationFunction

An activation function that returns the hyperbolic tangent of its input.

Deprecated

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

var BNNSActivationFunctionHardSigmoid: BNNSActivationFunction

An activation function that returns the hard sigmoid function of its input.

var BNNSActivationFunctionHardSwish: BNNSActivationFunction

An activation function that returns the hard swish function of its input.

var BNNSActivationFunctionIdentity: BNNSActivationFunctionDeprecated

var BNNSActivationFunctionLeakyRectifiedLinear: BNNSActivationFunctionDeprecated

var BNNSActivationFunctionLinearWithBias: BNNSActivationFunction

An activation function that returns its input multiplied by a scale and added to a bias.

var BNNSActivationFunctionLogSigmoid: BNNSActivationFunction

An activation function that returns the logarithm of the sigmoid function of its input.

var BNNSActivationFunctionLogSoftmax: BNNSActivationFunction

An activation function that returns the logarithm of the softmax function of its input.

var BNNSActivationFunctionPReLUPerChannel: BNNSActivationFunction

An activation function provides per-channel alpha values to Leaky Rectified Linear.

var BNNSActivationFunctionRectifiedLinear: BNNSActivationFunctionDeprecated

var BNNSActivationFunctionReLU6: BNNSActivationFunction

var BNNSActivationFunctionScaledTanh: BNNSActivationFunctionDeprecated

var BNNSActivationFunctionSELU: BNNSActivationFunction

An activation function that evaluates the scaled exponential linear units (SELU) on its input.

var BNNSActivationFunctionSigmoid: BNNSActivationFunctionDeprecated

var BNNSActivationFunctionSiLU: BNNSActivationFunction

An activation function that returns the sigmoid linear unit (SiLU) function of its input.

var BNNSActivationFunctionSoftplus: BNNSActivationFunction

An activation function that returns the softplus function of its input.

var BNNSActivationFunctionSoftShrink: BNNSActivationFunction

An activation function that returns zero when the absolute input is less than alpha, otherwise it returns its input minus alpha.

var BNNSActivationFunctionSoftsign: BNNSActivationFunction

An activation function that returns the softsign function of its input.

var BNNSActivationFunctionTanh: BNNSActivationFunctionDeprecated

var BNNSActivationFunctionTanhShrink: BNNSActivationFunction

An activation function that returns its input minus the hyperbolic tangent of its input.

var BNNSActivationFunctionThreshold: BNNSActivationFunction

An activation function that returns beta if its input is less than a specified threshold, otherwise it returns its input.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Activation layers

func BNNSFilterCreateVectorActivationLayer(UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSActivation>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?Deprecated

class ActivationLayer

A layer object that wraps an activation filter and manages its deinitialization.

Deprecated

struct BNNSActivation

A set of parameters that describe common activation functions.

struct BNNSLayerParametersActivation

A set of parameters that define an activation layer.

Deprecated

func BNNSFilterCreateLayerActivation(UnsafePointer&lt;BNNSLayerParametersActivation>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new activation layer.

Deprecated

func BNNSDirectApplyActivationBatch(UnsafePointer&lt;BNNSLayerParametersActivation>, UnsafePointer&lt;BNNSFilterParameters>?, Int, Int, Int) -> Int32

Applies an activation filter to a set of input objects, writing out the result to a set of output objects.

Deprecated

static func applyActivation(activation: BNNS.ActivationFunction, axes: [Int], input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, batchSize: Int, filterParameters: BNNSFilterParameters?) throws

Applies an activation function on the specified axes.

Deprecated

static func applyActivation(activation: BNNS.ActivationFunction, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, batchSize: Int, filterParameters: BNNSFilterParameters?) throws

Applies the specified activation function.

Deprecated

