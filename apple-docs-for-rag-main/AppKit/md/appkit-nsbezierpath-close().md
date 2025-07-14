

- AppKit
- NSBezierPath
-  close() 

Instance Method

# close()

Closes the most recently added subpath.

macOS

``` source
func close()
```

## Discussion

This method closes the current subpath by creating a line segment between the first and last points in the subpath. This method subsequently updates the current point to the end of the newly created line segment, which is also the first point in the now closed subpath.

## See Also

### Related Documentation

func fill()

Paints the region enclosed by the path.

### Constructing a Path

func move(to: NSPoint)

Moves the path’s current point to the specified location.

func line(to: NSPoint)

Appends a straight line to the path.

func curve(to: NSPoint, controlPoint1: NSPoint, controlPoint2: NSPoint)

Adds a Bezier cubic curve to the path.

func curve(to: NSPoint, controlPoint: NSPoint)

func relativeMove(to: NSPoint)

Moves the path’s current point to a new point whose location is the specified distance from the current point.

func relativeLine(to: NSPoint)

Appends a straight line segment to the path starting at the current point and moving towards the specified point, relative to the current location.

func relativeCurve(to: NSPoint, controlPoint1: NSPoint, controlPoint2: NSPoint)

Adds a Bezier cubic curve to the path from the current point to a new location, which is specified as a relative distance from the current point.

func relativeCurve(to: NSPoint, controlPoint: NSPoint)

