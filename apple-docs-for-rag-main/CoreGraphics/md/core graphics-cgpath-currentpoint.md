

- Core Graphics
- CGPath
-  currentPoint 

Instance Property

# currentPoint

Returns the current point in a graphics path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var currentPoint: CGPoint { get }
```

## Discussion

If the path is empty—that is, if it has no elements—this function returns CGPointZero (see CGGeometry). To determine whether a path is empty, use isEmpty.

## See Also

### Examining a Graphics Path

var boundingBox: CGRect

Returns the bounding box containing all points in a graphics path.

var boundingBoxOfPath: CGRect

Returns the bounding box of a graphics path.

func contains(CGPoint, using: CGPathFillRule, transform: CGAffineTransform) -> Bool

Returns whether the specified point is interior to the path.

var isEmpty: Bool

Indicates whether or not a graphics path is empty.

func isRect(UnsafeMutablePointer&lt;CGRect>?) -> Bool

Indicates whether or not a graphics path represents a rectangle.

