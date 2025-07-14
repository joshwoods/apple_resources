

- Core Graphics
- CGContext
-  boundingBoxOfPath 

Instance Property

# boundingBoxOfPath

Returns the smallest rectangle that contains the current path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var boundingBoxOfPath: CGRect { get }
```

## Discussion

The bounding box is the smallest rectangle completely enclosing all points in a path, including control points for Bézier cubic and quadratic curves.

## See Also

### Examining the Current Graphics Path

var currentPointOfPath: CGPoint

Returns the current point in a non-empty path.

var isPathEmpty: Bool

Indicates whether the current path contains any subpaths.

func pathContains(CGPoint, mode: CGPathDrawingMode) -> Bool

Checks to see whether the specified point is contained in the current path.

