

- AppKit
- NSBezierPath
-  curve(to:controlPoint:) 

Instance Method

# curve(to:controlPoint:)

macOS 14.0+

``` source
func curve(
    to endPoint: NSPoint,
    controlPoint: NSPoint
)
```

## See Also

### Constructing a Path

func move(to: NSPoint)

Moves the path’s current point to the specified location.

func line(to: NSPoint)

Appends a straight line to the path.

func curve(to: NSPoint, controlPoint1: NSPoint, controlPoint2: NSPoint)

Adds a Bezier cubic curve to the path.

func close()

Closes the most recently added subpath.

func relativeMove(to: NSPoint)

Moves the path’s current point to a new point whose location is the specified distance from the current point.

func relativeLine(to: NSPoint)

Appends a straight line segment to the path starting at the current point and moving towards the specified point, relative to the current location.

func relativeCurve(to: NSPoint, controlPoint1: NSPoint, controlPoint2: NSPoint)

Adds a Bezier cubic curve to the path from the current point to a new location, which is specified as a relative distance from the current point.

func relativeCurve(to: NSPoint, controlPoint: NSPoint)

