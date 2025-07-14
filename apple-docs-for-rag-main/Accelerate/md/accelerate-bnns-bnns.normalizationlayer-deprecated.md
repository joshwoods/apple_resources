

- Accelerate
- BNNS
-  BNNS.NormalizationLayer Deprecated

Class

# BNNS.NormalizationLayer

A layer object that wraps a normalization filter and manages its deinitialization.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+watchOS 7.0+visionOS

``` source
class NormalizationLayer
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating a Normalization Layer

convenience init?(type: BNNS.NormalizationType, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, beta: BNNSNDArrayDescriptor, gamma: BNNSNDArrayDescriptor, momentum: Float, epsilon: Float, activation: BNNS.ActivationFunction, filterParameters: BNNSFilterParameters?)

Returns a new normalization layer.

### Specifying a Normalization Type

enum NormalizationType

Constants that describe normalization types.

### Applying a Normalization Layer

func apply(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, for: BNNS.LearningPhase) throws

Applies the layer to a set of input objects, writing the result to a set of output objects.

func applyBackward(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, outputGradient: BNNSNDArrayDescriptor, generatingInputGradient: BNNSNDArrayDescriptor, generatingBetaGradient: BNNSNDArrayDescriptor?, generatingGammaGradient: BNNSNDArrayDescriptor?) throws

Applies the layer backward to generate input gradients.

### Specifying the Learning Phase

enum LearningPhase

Constants that describe the learning phase of a normalization operation.

## Relationships

### Inherits From

- BNNS.Layer

## See Also

### Normalization layers

struct BNNSLayerParametersNormalization

A structure that contains the parameters of a normalization layer.

Deprecated

func BNNSFilterCreateLayerNormalization(BNNSFilterType, UnsafePointer&lt;BNNSLayerParametersNormalization>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new normalization layer.

Deprecated

func BNNSNormalizationFilterApplyBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, Bool) -> Int32

Applies a normalization filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSNormalizationFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?) -> Int32

Applies a normalization filter backward to generate gradients.

Deprecated

