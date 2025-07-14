

- TabletopKit
- DieState
-  boundingBox 

Instance Property

# boundingBox

A 3D bounding box that encloses the die.

visionOS 2.0+

``` source
var boundingBox: Rect3D
```

## Discussion

This bounding box is object oriented, so remains the same regardless of the equipment orientation.

## See Also

### Rendering the equipment

var pose: TableVisualState.Pose2D

The 2D position and rotation of the equipment relative to the equipment parent, or table.

