

- AppKit
- NSBezierPath
-  controlPointBounds 

Instance Property

# controlPointBounds

The bounding box of the path, including any control points.

macOS

``` source
var controlPointBounds: NSRect { get }
```

## Discussion

This property contains the rectangle that encloses the receiver’s path. If the path contains curve segments, the bounding box encloses the control points of the curves as well as the curves themselves.

## See Also

### Querying a Path

var bounds: NSRect

The bounding box of the path.

var currentPoint: NSPoint

The current point (the trailing point or ending point in the most recently added segment).

var isEmpty: Bool

A Boolean value that indicates whether the path is empty.

