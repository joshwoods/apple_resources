

- Core ML
- MLMultiArrayShapeConstraint
-  enumeratedShapes 

Instance Property

# enumeratedShapes

Array of allowed shapes for a multiarray feature.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var enumeratedShapes: [[NSNumber]] { get }
```

## See Also

### Accessing the Constraints

var sizeRangeForDimension: [NSValue]

The allowable range for a dimention of the multiarray.

var type: MLMultiArrayShapeConstraintType

The type of the shape constraint.

enum MLMultiArrayShapeConstraintType

The possible types of shape constraints.

