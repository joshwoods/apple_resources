

- Accelerate
- BNNS
-  BNNS.FusedConvolutionNormalizationLayer Deprecated

Class

# BNNS.FusedConvolutionNormalizationLayer

A layer object that wraps a fused, convolution normalization layer and manages its deinitialization.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
class FusedConvolutionNormalizationLayer
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating a Fused Convolution Normalization Layer

convenience init?(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, convolutionWeights: BNNSNDArrayDescriptor, convolutionBias: BNNSNDArrayDescriptor?, convolutionStride: (x: Int, y: Int), convolutionDilationStride: (x: Int, y: Int), convolutionPadding: BNNS.ConvolutionPadding, normalization: BNNS.NormalizationType, normalizationBeta: BNNSNDArrayDescriptor, normalizationGamma: BNNSNDArrayDescriptor, normalizationMomentum: Float, normalizationEpsilon: Float, normalizationActivation: BNNS.ActivationFunction, filterParameters: BNNSFilterParameters?)

Returns a new fused, convolution normalization layer.

### Applying a Fused Layer

func apply(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, for: BNNS.LearningPhase) throws

Applies the layer to a set of input objects, writing the result to a set of output objects.

func applyBackward(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, outputGradient: BNNSNDArrayDescriptor, generatingInputGradient: BNNSNDArrayDescriptor, generatingParameterGradients: [BNNSNDArrayDescriptor]) throws

Applies the layer backward to generate input gradients.

### Specifying the Learning Phase

enum LearningPhase

Constants that describe the learning phase of a normalization operation.

## Relationships

### Inherits From

- BNNS.FusedLayer

## See Also

### Fused layers

protocol FusableLayerParametersDeprecated

class FusedParametersLayer

A layer object that wraps a fused layer and manages its deinitialization.

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

