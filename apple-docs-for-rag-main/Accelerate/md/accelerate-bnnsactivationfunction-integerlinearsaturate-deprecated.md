

- Accelerate
- BNNSActivationFunction
-  integerLinearSaturate Deprecated

Type Property

# integerLinearSaturate

An activation function that returns an arithmetic shift, preserving sign.

iOS 11.0+iPadOS 11.0+Mac CatalystmacOS 10.13+visionOSwatchOS 4.0+tvOS 11.0+

``` source
static var integerLinearSaturate: BNNSActivationFunction { get }
```

Deprecated

Use the BNNSGraph API instead.

## Discussion

Use integerLinearSaturate(scale:offset:shift:) to generate an integer linear saturate function.

## See Also

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

