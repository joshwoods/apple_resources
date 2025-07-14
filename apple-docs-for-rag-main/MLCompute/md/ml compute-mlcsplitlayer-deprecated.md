

- ML Compute
-  MLCSplitLayer Deprecated

Class

# MLCSplitLayer

A layer that splits a tensor value into a list of subtensors.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCSplitLayer
```

## Topics

### Creating Split Layers

convenience init(splitCount: Int, dimension: Int)

Creates a split layer with the number of splits and dimension you specify.

convenience init(splitSectionLengths: [Int], dimension: Int)

Creates a split layer with the lengths of each split section and dimension you specify.

### Inspecting Split Layers

var dimension: Int

The dimension or axis along which to split the tensor.

var splitCount: Int

The number of splits.

var splitSectionLengths: [Int]?

An array that contains the lengths of each split section.

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

class MLCSliceLayer

A layer that extracts a slice from a tensor.

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

