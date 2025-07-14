

- Core ML
-  MLMultiArrayShapeConstraintType 

Enumeration

# MLMultiArrayShapeConstraintType

The possible types of shape constraints.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
enum MLMultiArrayShapeConstraintType
```

## Topics

### Enumeration Cases

case enumerated

The constraint is an array of allowed shapes.

case range

The constraint is a set of ranges allowed for the array shape.

case unspecified

The constraint type is undefined.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing the Constraints

var enumeratedShapes: [[NSNumber]]

Array of allowed shapes for a multiarray feature.

var sizeRangeForDimension: [NSValue]

The allowable range for a dimention of the multiarray.

var type: MLMultiArrayShapeConstraintType

The type of the shape constraint.

