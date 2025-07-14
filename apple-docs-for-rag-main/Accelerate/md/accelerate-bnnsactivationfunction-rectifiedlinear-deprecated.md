

- Accelerate
- BNNSActivationFunction
-  rectifiedLinear Deprecated

Type Property

# rectifiedLinear

An activation function that returns its input when that is greater than or equal to zero, otherwise it returns zero.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+tvOS 10.0+watchOS 3.0+visionOS

``` source
static var rectifiedLinear: BNNSActivationFunction { get }
```

Deprecated

Use the BNNSGraph API instead.

## Discussion

This constant defines an activation function that returns values using the following operation:

```
0 if x=0
```

The following illustrates the output that the activation function generates from inputs in the range `-10...10`:

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

