

- Core Graphics
- CGPath
-  boundingBox 

Instance Property

# boundingBox

Returns the bounding box containing all points in a graphics path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var boundingBox: CGRect { get }
```

## Discussion

The bounding box is the smallest rectangle completely enclosing all points in the path, including control points for Bézier and quadratic curves. If the path is empty, this value is CGRectNull.

## See Also

### Examining a Graphics Path

var boundingBoxOfPath: CGRect

Returns the bounding box of a graphics path.

var currentPoint: CGPoint

Returns the current point in a graphics path.

func contains(CGPoint, using: CGPathFillRule, transform: CGAffineTransform) -> Bool

Returns whether the specified point is interior to the path.

var isEmpty: Bool

Indicates whether or not a graphics path is empty.

func isRect(UnsafeMutablePointer&lt;CGRect>?) -> Bool

Indicates whether or not a graphics path represents a rectangle.

