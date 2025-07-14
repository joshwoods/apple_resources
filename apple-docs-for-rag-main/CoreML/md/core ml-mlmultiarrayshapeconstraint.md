

- Core ML
-  MLMultiArrayShapeConstraint 

Class

# MLMultiArrayShapeConstraint

The lists of shapes or ranges of shapes that constrain a multiarray feature.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class MLMultiArrayShapeConstraint
```

## Topics

### Accessing the Constraints

var enumeratedShapes: [[NSNumber]]

Array of allowed shapes for a multiarray feature.

var sizeRangeForDimension: [NSValue]

The allowable range for a dimention of the multiarray.

var type: MLMultiArrayShapeConstraintType

The type of the shape constraint.

enum MLMultiArrayShapeConstraintType

The possible types of shape constraints.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Accessing the Constraints

var shape: [NSNumber]

The shape of the multi array.

var dataType: MLMultiArrayDataType

The type for the multi array.

var shapeConstraint: MLMultiArrayShapeConstraint

The constraint on the shape of the multiarray.

