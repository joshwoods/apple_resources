

- ML Compute
-  MLCPaddingLayer Deprecated

Class

# MLCPaddingLayer

A layer that pads a tensor with the padding sizes you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCPaddingLayer
```

## Topics

### Creating Padding Layers

convenience init(reflectionPadding: [Int])

Creates a padding layer with the reflection padding sizes you specify.

convenience init(symmetricPadding: [Int])

Creates a padding layer with the symmetric padding sizes you specify.

convenience init(zeroPadding: [Int])

Creates a padding layer with the zero padding sizes you specify.

convenience init(constantPadding: [Int], constantValue: Float)

Creates a padding layer with the constant padding sizes and constant value you specify.

### Inspecting Padding Layers

var paddingType: MLCPaddingType

The padding type.

var paddingLeft: Int

The left padding size.

var paddingRight: Int

The right padding size.

var paddingTop: Int

The top padding size.

var paddingBottom: Int

The bottom padding size.

var constantValue: Float

The constant value you use if padding type is constant.

## Relationships

### Inherits From

- MLCLayer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
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

class MLCScatterLayer

A layer that updates the output at an index you specify.

Deprecated

class MLCSelectionLayer

A layer for selecting elements from two tensors.

Deprecated

class MLCGatherLayer

A layer that fetches data at the locations you specify.

Deprecated

