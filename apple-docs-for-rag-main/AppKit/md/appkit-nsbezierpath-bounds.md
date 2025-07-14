

- AppKit
- NSBezierPath
-  bounds 

Instance Property

# bounds

The bounding box of the path.

macOS

``` source
var bounds: NSRect { get }
```

## Discussion

This property contains the rectangle that encloses the path of the receiver. If the path contains curve segments, the bounding box encloses the curve but may not enclose the control points used to calculate the curve.

If the path is empty, accessing this property raises genericException.

## See Also

### Querying a Path

var controlPointBounds: NSRect

The bounding box of the path, including any control points.

var currentPoint: NSPoint

The current point (the trailing point or ending point in the most recently added segment).

var isEmpty: Bool

A Boolean value that indicates whether the path is empty.

