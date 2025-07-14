

- Accelerate
- BNNS
-  BNNS.FusedParametersLayer Deprecated

Class

# BNNS.FusedParametersLayer

A layer object that wraps a fused layer and manages its deinitialization.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
class FusedParametersLayer
```

Deprecated

Use the BNNSGraph API instead.

## Overview

Use a BNNS.FusedParametersLayer instance to fuse component layers with the following configurations:

- Convolution → Normalization

- Fully Connected → Normalization

- Transposed Convolution → Normalization

- Convolution → Quantization

- Fully Connected → Quantization

- Transposed Convolution → Quantization

- Arithmetic → Normalization

## Topics

### Creating a Fused Parameters Layer

convenience init?(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, fusedLayerParameters: [any FusableLayerParameters], filterParameters: BNNSFilterParameters?)

Creates a new fused layer from an array of layer parameters.

convenience init?(inputA: BNNSNDArrayDescriptor, inputB: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, fusedLayerParameters: [any FusableLayerParameters], filterParameters: BNNSFilterParameters?)

Creates a new fused layer from an array of layer parameters, where the first layer accepts two inputs.

convenience init?(inputA: BNNSNDArrayDescriptor, inputB: BNNSNDArrayDescriptor, inputC: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, fusedLayerParameters: [any FusableLayerParameters], filterParameters: BNNSFilterParameters?)

Creates a new fused layer from an array of layer parameters, where the first layer accepts three inputs.

### Specifying a Layer Parameter

struct FusedUnaryArithmeticParameters

A structure that contains the parameters for a fused unary arithmetic layer.

struct FusedBinaryArithmeticParameters

A structure that contains the parameters for a fused binary arithmetic layer.

struct FusedTernaryArithmeticParameters

A structure that contains the parameters for a fused ternary arithmetic layer.

struct FusedConvolutionParameters

A structure that contains the parameters for a fused convolution layer.

struct FusedQuantizationParameters

A structure that contains the parameters for a fused quantization layer.

struct FusedDequantizationParameters

A structure that contains the parameters for a fused dequantization layer.

struct FusedFullyConnectedParameters

A structure that contains the parameters for a fused fully connected layer.

struct FusedNormalizationParameters

A structure that contains the parameters for a fused normalization layer.

### Applying a Fused Parameters Layer

func apply(batchSize: Int, inputA: BNNSNDArrayDescriptor, inputB: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, for: BNNS.LearningPhase) throws

Applies the layer to a set of input objects and writes the result to a set of output objects, where the first layer accepts two inputs.

func apply(batchSize: Int, inputA: BNNSNDArrayDescriptor, inputB: BNNSNDArrayDescriptor, inputC: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, for: BNNS.LearningPhase) throws

Applies the layer to a set of input objects and writes the result to a set of output objects, where the first layer accepts two inputs.

func applyBackward(batchSize: Int, inputA: BNNSNDArrayDescriptor, inputB: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, outputGradient: BNNSNDArrayDescriptor, generatingInputAGradient: BNNSNDArrayDescriptor, generatingInputBGradient: BNNSNDArrayDescriptor, generatingParameterGradients: [BNNSNDArrayDescriptor]) throws

Applies the layer backward to generate input gradients, where the first layer accepts two inputs.

func applyBackward(batchSize: Int, inputA: BNNSNDArrayDescriptor, inputB: BNNSNDArrayDescriptor, inputC: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, outputGradient: BNNSNDArrayDescriptor, generatingInputAGradient: BNNSNDArrayDescriptor, generatingInputBGradient: BNNSNDArrayDescriptor, generatingInputCGradient: BNNSNDArrayDescriptor, generatingParameterGradients: [BNNSNDArrayDescriptor]) throws

Applies the layer backward to generate input gradients, where the first layer accepts three inputs.

## Relationships

### Inherits From

- BNNS.FusedLayer

## See Also

### Fused layers

protocol FusableLayerParametersDeprecated

class FusedConvolutionNormalizationLayer

A layer object that wraps a fused, convolution normalization layer and manages its deinitialization.

Deprecated

class FusedFullyConnectedNormalizationLayer

A layer object that wraps a fused, fully connected normalization layer and manages its deinitialization.

Deprecated

struct BNNSFilterType

Constants that define the component filters of a fused layer.

func BNNSFilterCreateFusedLayer(Int, UnsafePointer&lt;BNNSFilterType>, UnsafeMutablePointer&lt;UnsafeRawPointer>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new fused layer.

Deprecated

func BNNSFusedFilterApplyBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, Bool) -> Int32

Applies a fused filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSFusedFilterApplyMultiInputBatch(BNNSFilter?, Int, Int, UnsafeMutablePointer&lt;UnsafeRawPointer>, UnsafePointer&lt;Int>, UnsafeMutableRawPointer, Int, Bool) -> Int32

Applies a multiple-input fused filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSFusedFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?>?) -> Int32

Applies a fused filter backward to generate input gradients.

Deprecated

func BNNSFusedFilterApplyBackwardMultiInputBatch(BNNSFilter?, Int, Int, UnsafeMutablePointer&lt;UnsafeRawPointer?>?, UnsafePointer&lt;Int>?, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>>, UnsafePointer&lt;Int>, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?>?) -> Int32

Applies a multiple-input fused filter backward to generate input gradients.

Deprecated

