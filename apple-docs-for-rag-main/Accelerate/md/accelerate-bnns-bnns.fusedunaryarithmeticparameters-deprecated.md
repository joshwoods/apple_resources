

- Accelerate
- BNNS
-  BNNS.FusedUnaryArithmeticParameters Deprecated

Structure

# BNNS.FusedUnaryArithmeticParameters

A structure that contains the parameters for a fused unary arithmetic layer.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
struct FusedUnaryArithmeticParameters
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating a Fused Arithmetic Parameters Structure

init(inputDescriptorType: BNNS.DescriptorType, outputDescriptorType: BNNS.DescriptorType, function: BNNS.ArithmeticUnaryFunction)

Returns a new fused unary arithmetic parameters structure.

### Inspecting the Properties of a Fused Arithmetic Parameters Structure

var inputDescriptorType: BNNS.DescriptorType

The descriptor type of the input.

var outputDescriptorType: BNNS.DescriptorType

The descriptor type of the output.

var function: BNNS.ArithmeticUnaryFunction

The arithmetic function.

## Relationships

### Conforms To

- FusableLayerParameters

## See Also

### Specifying a Layer Parameter

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

struct FusedNormalizationParameters

A structure that contains the parameters for a fused normalization layer.

Deprecated

