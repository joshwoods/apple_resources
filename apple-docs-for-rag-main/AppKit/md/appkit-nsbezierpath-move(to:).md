

- AppKit
- NSBezierPath
-  move(to:) 

Instance Method

# move(to:)

Moves the path’s current point to the specified location.

macOS

``` source
func move(to point: NSPoint)
```

## Parameters 

`point`  

A point in the current coordinate system.

## Discussion

This method implicitly closes the current subpath (if any) and sets the current point to the value in `aPoint`. When closing the previous subpath, this method does not cause a line to be created from the first and last points in the subpath.

For many path operations, you must invoke this method before issuing any commands that cause a line or curve segment to be drawn.

## See Also

### Constructing a Path

func line(to: NSPoint)

Appends a straight line to the path.

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

