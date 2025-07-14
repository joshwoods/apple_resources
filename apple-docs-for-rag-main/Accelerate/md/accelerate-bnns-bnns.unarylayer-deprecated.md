

- Accelerate
- BNNS
-  BNNS.UnaryLayer Deprecated

Class

# BNNS.UnaryLayer

The base class for layers that accept a single input.

iOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+Mac Catalyst

``` source
class UnaryLayer
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Applying a Unary Layer

func apply(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor) throws

Applies the layer to a set of input objects, writing the result to a set of output objects.

func applyBackward(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, outputGradient: BNNSNDArrayDescriptor, generatingInputGradient: BNNSNDArrayDescriptor) throws

Applies the layer backward to generate input gradients.

## Relationships

### Inherits From

- BNNS.Layer

### Inherited By

- BNNS.ActivationLayer
- BNNS.ConvolutionLayer
- BNNS.DropoutLayer
- BNNS.GramLayer
- BNNS.PaddingLayer
- BNNS.PermuteLayer
- BNNS.ReductionLayer
- BNNS.ResizeLayer

## See Also

### Base Classes

class Layer

The base class for layer objects that wrap filters and manage deinitialization.

Deprecated

class BinaryLayer

The base class for layers that accept two inputs.

Deprecated

