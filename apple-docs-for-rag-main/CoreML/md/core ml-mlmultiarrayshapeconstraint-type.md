

- Core ML
- MLMultiArrayShapeConstraint
-  type 

Instance Property

# type

The type of the shape constraint.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var type: MLMultiArrayShapeConstraintType { get }
```

## See Also

### Accessing the Constraints

var enumeratedShapes: [[NSNumber]]

Array of allowed shapes for a multiarray feature.

var sizeRangeForDimension: [NSValue]

The allowable range for a dimention of the multiarray.

enum MLMultiArrayShapeConstraintType

The possible types of shape constraints.

