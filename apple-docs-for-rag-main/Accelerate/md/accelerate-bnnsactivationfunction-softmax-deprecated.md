

- Accelerate
- BNNSActivationFunction
-  softmax Deprecated

Type Property

# softmax

An activation function that returns the softmax function of its input.

iOS 11.0+iPadOS 11.0+Mac CatalystmacOS 10.13+tvOS 11.0+visionOSwatchOS 4.0+

``` source
static var softmax: BNNSActivationFunction { get }
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

static var tanh: BNNSActivationFunction

An activation function that returns the hyperbolic tangent of its input.

Deprecated

