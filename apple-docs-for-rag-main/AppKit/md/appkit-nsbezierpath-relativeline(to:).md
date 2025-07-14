

- AppKit
- NSBezierPath
-  relativeLine(to:) 

Instance Method

# relativeLine(to:)

Appends a straight line segment to the path starting at the current point and moving towards the specified point, relative to the current location.

macOS

``` source
func relativeLine(to point: NSPoint)
```

## Parameters 

`point`  

A point whose coordinates are interpreted as a relative offset from the current point.

## Discussion

The destination point is relative to the current point. For example, if the current point is (1, 1) and `aPoint` contains the value (1, 2), a line segment is created between the points (1, 1) and (2, 3).

You must set the path’s current point (using the move(to:) method or through the creation of a preceding line or curve segment) before you invoke this method. If the path is empty, this method raises an genericException exception.

## See Also

### Constructing a Path

func move(to: NSPoint)

Moves the path’s current point to the specified location.

func line(to: NSPoint)

Appends a straight line to the path.

func curve(to: NSPoint, controlPoint1: NSPoint, controlPoint2: NSPoint)

Adds a Bezier cubic curve to the path.

func curve(to: NSPoint, controlPoint: NSPoint)

func close()

Closes the most recently added subpath.

func relativeMove(to: NSPoint)

Moves the path’s current point to a new point whose location is the specified distance from the current point.

func relativeCurve(to: NSPoint, controlPoint1: NSPoint, controlPoint2: NSPoint)

Adds a Bezier cubic curve to the path from the current point to a new location, which is specified as a relative distance from the current point.

func relativeCurve(to: NSPoint, controlPoint: NSPoint)

