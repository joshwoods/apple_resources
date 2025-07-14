

- Accelerate
- BNNS
-  BNNS.BinaryLayer Deprecated

Class

# BNNS.BinaryLayer

The base class for layers that accept two inputs.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
class BinaryLayer
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Applying a Binary Layer

func apply(batchSize: Int, inputA: BNNSNDArrayDescriptor, inputB: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor) throws

Applies the layer to a set of input object pairs, writing the result to a set of output objects.

func applyBackward(batchSize: Int, inputA: BNNSNDArrayDescriptor, inputB: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, outputGradient: BNNSNDArrayDescriptor, generatingInputAGradient: BNNSNDArrayDescriptor, generatingInputBGradient: BNNSNDArrayDescriptor) throws

Applies the layer backward to generate input gradients.

## Relationships

### Inherits From

- BNNS.Layer

## See Also

### Base Classes

class Layer

The base class for layer objects that wrap filters and manage deinitialization.

Deprecated

class UnaryLayer

The base class for layers that accept a single input.

Deprecated

