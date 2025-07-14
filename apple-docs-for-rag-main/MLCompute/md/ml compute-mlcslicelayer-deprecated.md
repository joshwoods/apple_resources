

- ML Compute
-  MLCSliceLayer Deprecated

Class

# MLCSliceLayer

A layer that extracts a slice from a tensor.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCSliceLayer
```

## Overview

The framework supports positive stride.

Use a slice layer to slice a given source. Slicing won’t decrease the tensor dimension. The start, end, and stride vectors must be of the same size, equal to the source tensor dimension.

## Topics

### Creating Slice Layers

convenience init?(start: [Int], end: [Int], stride: [Int]?)

Creates a slice layer with the start, end, and stride you specify.

### Inspecting Slice Layers

var start: [Int]

The start vector.

var end: [Int]

The end vector.

var stride: [Int]?

The stride vector.

## Relationships

### Inherits From

- MLCLayer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Transformation Layers

class MLCTransposeLayer

A layer that permutes the dimensions you specify.

Deprecated

class MLCConcatenationLayer

A layer that combines tensors into a single tensor.

Deprecated

class MLCReshapeLayer

A layer that reshapes a tensor with the shape you specify.

Deprecated

class MLCSplitLayer

A layer that splits a tensor value into a list of subtensors.

Deprecated

class MLCPaddingLayer

A layer that pads a tensor with the padding sizes you specify.

Deprecated

class MLCScatterLayer

A layer that updates the output at an index you specify.

Deprecated

class MLCSelectionLayer

A layer for selecting elements from two tensors.

Deprecated

class MLCGatherLayer

A layer that fetches data at the locations you specify.

Deprecated

