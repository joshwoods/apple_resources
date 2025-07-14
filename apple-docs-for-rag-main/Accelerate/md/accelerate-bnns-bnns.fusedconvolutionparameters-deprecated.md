

- Accelerate
- BNNS
-  BNNS.FusedConvolutionParameters Deprecated

Structure

# BNNS.FusedConvolutionParameters

A structure that contains the parameters for a fused convolution layer.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
struct FusedConvolutionParameters
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating a Fused Convolution Parameters Structure

init(type: BNNS.ConvolutionType, weights: BNNSNDArrayDescriptor, bias: BNNSNDArrayDescriptor?, stride: (x: Int, y: Int), dilationStride: (x: Int, y: Int), groupSize: Int, padding: BNNS.ConvolutionPadding)

Returns a new fused convolution parameters structure.

### Inspecting the Properties of a Fused Convolution Parameters Structure

var type: BNNS.ConvolutionType

An enumeration that specifies the convolution type.

var weights: BNNSNDArrayDescriptor

The descriptor of the weights.

var bias: BNNSNDArrayDescriptor?

The descriptor of the bias.

var stride: (x: Int, y: Int)

The width and height increments of the input image.

var dilationStride: (x: Int, y: Int)

The width and height increments between elements in the input image during convolution.

var groupSize: Int

The convolution group size.

var padding: BNNS.ConvolutionPadding

The number of zeros that the operation virtually adds to the edges of the input.

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

