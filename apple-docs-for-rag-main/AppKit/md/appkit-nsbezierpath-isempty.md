

- AppKit
- NSBezierPath
-  isEmpty 

Instance Property

# isEmpty

A Boolean value that indicates whether the path is empty.

macOS

``` source
var isEmpty: Bool { get }
```

## Discussion

The value of this property is true if the path contains no elements, or false if it contains at least one element.

## See Also

### Querying a Path

var bounds: NSRect

The bounding box of the path.

var controlPointBounds: NSRect

The bounding box of the path, including any control points.

var currentPoint: NSPoint

The current point (the trailing point or ending point in the most recently added segment).

