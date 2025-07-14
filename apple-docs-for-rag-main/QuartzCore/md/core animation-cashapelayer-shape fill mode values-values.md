

- Core Animation
- CAShapeLayer
-  Shape Fill Mode Values 

API Collection

# Shape Fill Mode Values

These constants specify the possible fill modes for fillRule.

## Topics

### Constants

static let nonZero: CAShapeLayerFillRule

Specifies the non-zero winding rule. Count each left-to-right path as +1 and each right-to-left path as -1. If the sum of all crossings is 0, the point is outside the path. If the sum is nonzero, the point is inside the path and the region containing it is filled.

static let evenOdd: CAShapeLayerFillRule

Specifies the even-odd winding rule. Count the total number of path crossings. If the number of crossings is even, the point is outside the path. If the number of crossings is odd, the point is inside the path and the region containing it should be filled.

## See Also

### Constants

Line Join Values

These constants specify the shape of the joints between connected segments of a stroked path.

Line Cap Values

These constants specify the shape of endpoints for an open path when stroked.

