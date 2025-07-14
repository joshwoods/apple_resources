

- ML Compute
-  MLCConcatenationLayer Deprecated

Class

# MLCConcatenationLayer

A layer that combines tensors into a single tensor.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCConcatenationLayer
```

## Topics

### Creating Concatenation Layers

convenience init()

Creates a concatenation layer with a dimension value of 1, which typically represents feature channels.

convenience init(dimension: Int)

Creates a concatenation layer with the dimension you specify.

### Inspecting Concatenation Layers

var dimension: Int

The dimension, or axis, along which you concatenate tensors.

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

class MLCReshapeLayer

A layer that reshapes a tensor with the shape you specify.

Deprecated

class MLCSliceLayer

A layer that extracts a slice from a tensor.

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

