

- Core Graphics
- CGPath
-  boundingBoxOfPath 

Instance Property

# boundingBoxOfPath

Returns the bounding box of a graphics path.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var boundingBoxOfPath: CGRect { get }
```

## Discussion

The path bounding box is the smallest rectangle completely enclosing all points in the path but not including control points for Bézier and quadratic curves. If the path is empty, this value is CGRectNull.

## See Also

### Examining a Graphics Path

var boundingBox: CGRect

Returns the bounding box containing all points in a graphics path.

var currentPoint: CGPoint

Returns the current point in a graphics path.

func contains(CGPoint, using: CGPathFillRule, transform: CGAffineTransform) -> Bool

Returns whether the specified point is interior to the path.

var isEmpty: Bool

Indicates whether or not a graphics path is empty.

func isRect(UnsafeMutablePointer&lt;CGRect>?) -> Bool

Indicates whether or not a graphics path represents a rectangle.

