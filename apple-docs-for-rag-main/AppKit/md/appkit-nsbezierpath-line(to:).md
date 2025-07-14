

- AppKit
- NSBezierPath
-  line(to:) 

Instance Method

# line(to:)

Appends a straight line to the path.

macOS

``` source
func line(to point: NSPoint)
```

## Parameters 

`point`  

The destination point of the line segment, specified in the current coordinate system.

## Discussion

This method creates a straight line segment starting at the current point and ending at the point specified by the `aPoint` parameter. The current point is the last point in the receiver’s most recently added segment.

You must set the path’s current point (using the move(to:) method or through the creation of a preceding line or curve segment) before you invoke this method. If the path is empty, this method raises an genericException exception.

## See Also

### Constructing a Path

func move(to: NSPoint)

Moves the path’s current point to the specified location.

func curve(to: NSPoint, controlPoint1: NSPoint, controlPoint2: NSPoint)

Adds a Bezier cubic curve to the path.

func curve(to: NSPoint, controlPoint: NSPoint)

func close()

Closes the most recently added subpath.

func relativeMove(to: NSPoint)

Moves the path’s current point to a new point whose location is the specified distance from the current point.

func relativeLine(to: NSPoint)

Appends a straight line segment to the path starting at the current point and moving towards the specified point, relative to the current location.

func relativeCurve(to: NSPoint, controlPoint1: NSPoint, controlPoint2: NSPoint)

Adds a Bezier cubic curve to the path from the current point to a new location, which is specified as a relative distance from the current point.

func relativeCurve(to: NSPoint, controlPoint: NSPoint)

