

- Accelerate
- BNNS
-  BNNS.FusedLayer Deprecated

Class

# BNNS.FusedLayer

The base class for fused convolution-normalization and fully connected-normalization layers.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
class FusedLayer
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Applying a Fused Layer

func apply(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, for: BNNS.LearningPhase) throws

Applies the layer to a set of input objects, writing the result to a set of output objects.

func applyBackward(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, outputGradient: BNNSNDArrayDescriptor, generatingInputGradient: BNNSNDArrayDescriptor, generatingParameterGradients: [BNNSNDArrayDescriptor]) throws

Applies the layer backward to generate input gradients.

## Relationships

### Inherits From

- BNNS.Layer

### Inherited By

- BNNS.FusedConvolutionNormalizationLayer
- BNNS.FusedFullyConnectedNormalizationLayer
- BNNS.FusedParametersLayer

