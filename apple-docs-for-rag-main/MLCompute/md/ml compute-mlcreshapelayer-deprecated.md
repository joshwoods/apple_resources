

- ML Compute
-  MLCReshapeLayer Deprecated

Class

# MLCReshapeLayer

A layer that reshapes a tensor with the shape you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCReshapeLayer
```

## Topics

### Creating Reshape Layers

convenience init?(shape: [Int])

Creates a reshape layer with the shape you specify.

### Inspecting Reshape Layers

var shape: [Int]

An array that contains the size of each dimension.

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

