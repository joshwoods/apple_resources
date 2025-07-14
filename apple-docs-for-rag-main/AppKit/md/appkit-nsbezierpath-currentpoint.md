

- AppKit
- NSBezierPath
-  currentPoint 

Instance Property

# currentPoint

The current point (the trailing point or ending point in the most recently added segment).

macOS

``` source
var currentPoint: NSPoint { get }
```

## Discussion

This property contains the point from which the next drawn line or curve segment begins. If the path is empty, accessing this property raises genericException.

## See Also

### Related Documentation

func curve(to: NSPoint, controlPoint1: NSPoint, controlPoint2: NSPoint)

Adds a Bezier cubic curve to the path.

func close()

Closes the most recently added subpath.

func move(to: NSPoint)

Moves the path’s current point to the specified location.

func line(to: NSPoint)

Appends a straight line to the path.

### Querying a Path

var bounds: NSRect

The bounding box of the path.

var controlPointBounds: NSRect

The bounding box of the path, including any control points.

var isEmpty: Bool

A Boolean value that indicates whether the path is empty.

