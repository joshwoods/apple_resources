

- Accelerate
- BNNS
-  BNNS.FusedFullyConnectedParameters Deprecated

Structure

# BNNS.FusedFullyConnectedParameters

A structure that contains the parameters for a fused fully connected layer.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
struct FusedFullyConnectedParameters
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating a Fused Fully Connected Parameters Structure

init(weights: BNNSNDArrayDescriptor, bias: BNNSNDArrayDescriptor?)

Returns a new fused dequantization parameters structure.

### Inspecting the Properties of a Fused Fully Connected Parameters Structure

var weights: BNNSNDArrayDescriptor

The descriptor of the weights.

var bias: BNNSNDArrayDescriptor?

The descriptor of the bias.

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

struct FusedNormalizationParameters

A structure that contains the parameters for a fused normalization layer.

Deprecated

