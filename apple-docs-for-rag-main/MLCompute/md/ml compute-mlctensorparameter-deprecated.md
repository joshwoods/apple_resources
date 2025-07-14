

- ML Compute
-  MLCTensorParameter Deprecated

Class

# MLCTensorParameter

A tensor parameter object.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCTensorParameter
```

## Overview

Use a tensor parameter to describe input tensors that the optimizer updates during training.

## Topics

### Creating Tensor Parameters

convenience init(tensor: MLCTensor)

Creates a tensor parameter with the tensor you specify.

convenience init(tensor: MLCTensor, optimizerData: [MLCTensorData]?)

Creates a tensor parameter with the tensor and optimizer data you specify.

### Inspecting Tensor Parameters

var tensor: MLCTensor

The underlying tensor.

var isUpdatable: Bool

A Boolean that indicates whether this tensor parameter is updatable.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Creating Training Graphs

convenience init(graphObjects: [MLCGraph], lossLayer: MLCLayer?, optimizer: MLCOptimizer?)

Creates a training graph with the layers from the graph objects, loss layer, and optimizer you specify.

Deprecated

Optimizers

Create an optimizer to use with the training graph.

