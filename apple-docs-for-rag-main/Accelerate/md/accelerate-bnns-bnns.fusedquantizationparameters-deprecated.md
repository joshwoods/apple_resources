

- Accelerate
- BNNS
-  BNNS.FusedQuantizationParameters Deprecated

Structure

# BNNS.FusedQuantizationParameters

A structure that contains the parameters for a fused quantization layer.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+Mac Catalyst

``` source
struct FusedQuantizationParameters
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating a Fused Quantization Parameters Structure

init(scale: BNNSNDArrayDescriptor?, bias: BNNSNDArrayDescriptor?)

Returns a new fused quantization parameters structure.

### Inspecting the Properties of a Fused Quantization Parameters Structure

var scale: BNNSNDArrayDescriptor?

The descriptor of the scale.

var bias: BNNSNDArrayDescriptor?

The descriptor of the bias.

var axis: Int?

The index of the axis on which the function applies scale and bias.

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

struct FusedDequantizationParameters

A structure that contains the parameters for a fused dequantization layer.

Deprecated

struct FusedFullyConnectedParameters

A structure that contains the parameters for a fused fully connected layer.

Deprecated

struct FusedNormalizationParameters

A structure that contains the parameters for a fused normalization layer.

Deprecated

