

- ML Compute
-  MLCScatterLayer Deprecated

Class

# MLCScatterLayer

A layer that updates the output at an index you specify.

iOS 14.5–17.4DeprecatediPadOS 14.5–17.4DeprecatedMac Catalyst 14.5–17.4DeprecatedmacOS 11.3–14.3DeprecatedtvOS 14.5–17.4Deprecated

``` source
class MLCScatterLayer
```

## Topics

### Creating Scatter Layers

convenience init?(dimension: Int, reductionType: MLCReductionType)

Creates a scatter layer with the dimension and reduction type you specify.

### Inspecting Scatter Layers

var dimension: Int

The dimension to index.

var reductionType: MLCReductionType

The reduction type that applies to all values in the source tensor.

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

class MLCSplitLayer

A layer that splits a tensor value into a list of subtensors.

Deprecated

class MLCPaddingLayer

A layer that pads a tensor with the padding sizes you specify.

Deprecated

class MLCSelectionLayer

A layer for selecting elements from two tensors.

Deprecated

class MLCGatherLayer

A layer that fetches data at the locations you specify.

Deprecated

