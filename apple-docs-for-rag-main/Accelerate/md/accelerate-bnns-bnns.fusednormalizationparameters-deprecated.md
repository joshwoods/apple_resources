

- Accelerate
- BNNS
-  BNNS.FusedNormalizationParameters Deprecated

Structure

# BNNS.FusedNormalizationParameters

A structure that contains the parameters for a fused normalization layer.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
struct FusedNormalizationParameters
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating a Fused Normalization Parameters Structure

init(type: BNNS.NormalizationType, beta: BNNSNDArrayDescriptor?, gamma: BNNSNDArrayDescriptor?, momentum: Float, epsilon: Float, activation: BNNS.ActivationFunction)

Returns a new fused normalization parameters structure.

### Inspecting the Properties of a Fused Normalization Parameters Structure

var type: BNNS.NormalizationType

An enumeration that specifies the normalization type.

var beta: BNNSNDArrayDescriptor?

The descriptor of the beta.

var gamma: BNNSNDArrayDescriptor?

The descriptor of the gamma.

var momentum: Float

A value, between 0 and 1, the normalization operation uses to update the moving mean and moving variance during training.

var epsilon: Float

The epsilon in the computation of the standard deviation.

var activation: BNNS.ActivationFunction

The activation function that the layer applies to the output.

## Relationships

### Conforms To

- FusableLayerParameters

## See Also

### Specifying a Layer Parameter

struct FusedUnaryArithmeticParameters

A structure that contains the parameters for a fused unary arithmetic layer.

Deprecated

struct FusedBinaryArithmeticParameters

A structure that contains the parameters for a fused binary arithmetic layer.

Deprecated

struct FusedTernaryArithmeticParameters

A structure that contains the parameters for a fused ternary arithmetic layer.

Deprecated

struct FusedConvolutionParameters

A structure that contains the parameters for a fused convolution layer.

Deprecated

struct FusedQuantizationParameters

A structure that contains the parameters for a fused quantization layer.

Deprecated

struct FusedDequantizationParameters

A structure that contains the parameters for a fused dequantization layer.

Deprecated

struct FusedFullyConnectedParameters

A structure that contains the parameters for a fused fully connected layer.

Deprecated

