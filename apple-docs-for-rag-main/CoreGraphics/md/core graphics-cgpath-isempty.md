

- Core Graphics
- CGPath
-  isEmpty 

Instance Property

# isEmpty

Indicates whether or not a graphics path is empty.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var isEmpty: Bool { get }
```

## Discussion

An empty path contains no elements.

## See Also

### Examining a Graphics Path

var boundingBox: CGRect

Returns the bounding box containing all points in a graphics path.

var boundingBoxOfPath: CGRect

Returns the bounding box of a graphics path.

var currentPoint: CGPoint

Returns the current point in a graphics path.

func contains(CGPoint, using: CGPathFillRule, transform: CGAffineTransform) -> Bool

Returns whether the specified point is interior to the path.

func isRect(UnsafeMutablePointer&lt;CGRect>?) -> Bool

Indicates whether or not a graphics path represents a rectangle.

