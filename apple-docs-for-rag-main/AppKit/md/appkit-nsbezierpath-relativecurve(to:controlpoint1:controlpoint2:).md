

- AppKit
- NSBezierPath
-  relativeCurve(to:controlPoint1:controlPoint2:) 

Instance Method

# relativeCurve(to:controlPoint1:controlPoint2:)

Adds a Bezier cubic curve to the path from the current point to a new location, which is specified as a relative distance from the current point.

macOS

``` source
func relativeCurve(
    to endPoint: NSPoint,
    controlPoint1: NSPoint,
    controlPoint2: NSPoint
)
```

## Parameters 

`endPoint`  

The destination point of the curve segment, interpreted as a relative offset from the current point.

`controlPoint1`  

The point that determines the shape of the curve near the current point, interpreted as a relative offset from the current point.

`controlPoint2`  

The point that determines the shape of the curve near the destination point, interpreted as a relative offset from the current point.

## Discussion

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

func relativeLine(to: NSPoint)

Appends a straight line segment to the path starting at the current point and moving towards the specified point, relative to the current location.

func relativeCurve(to: NSPoint, controlPoint: NSPoint)

