

- Accelerate
- BNNS
-  BNNS.FusedTernaryArithmeticParameters Deprecated

Structure

# BNNS.FusedTernaryArithmeticParameters

A structure that contains the parameters for a fused ternary arithmetic layer.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+visionOSwatchOS 8.0+tvOS 15.0+

``` source
struct FusedTernaryArithmeticParameters
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating a Fused Arithmetic Parameters Structure

init(inputADescriptorType: BNNS.DescriptorType, inputBDescriptorType: BNNS.DescriptorType, inputCDescriptorType: BNNS.DescriptorType, outputDescriptorType: BNNS.DescriptorType, function: BNNS.ArithmeticTernaryFunction)

Returns a new fused ternary arithmetic parameters structure.

### Inspecting the Properties of a Fused Arithmetic Parameters Structure

var function: BNNS.ArithmeticTernaryFunction

The arithmetic function.

var inputADescriptorType: BNNS.DescriptorType

The descriptor type of the first input.

var inputBDescriptorType: BNNS.DescriptorType

The descriptor type of the second input.

var inputCDescriptorType: BNNS.DescriptorType

The descriptor type of the third input.

var outputDescriptorType: BNNS.DescriptorType

The descriptor type of the output.

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

