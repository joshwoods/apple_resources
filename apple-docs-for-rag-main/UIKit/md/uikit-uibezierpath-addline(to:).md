

- UIKit
- UIBezierPath
-  addLine(to:) 

Instance Method

# addLine(to:)

Appends a straight line to the path.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func addLine(to point: CGPoint)
```

## Parameters 

`point`  

The destination point of the line segment, specified in the current coordinate system.

## Discussion

This method creates a straight line segment starting at the current point and ending at the point specified by the `point` parameter. After adding the line segment, this method updates the current point to the value in `point`.

You must set the path’s current point (using the move(to:) method or through the previous creation of a line or curve segment) before you call this method. If the path is empty, this method does nothing.

## See Also

### Constructing a path

func move(to: CGPoint)

Moves the path’s current point to the specified location.

func addArc(withCenter: CGPoint, radius: CGFloat, startAngle: CGFloat, endAngle: CGFloat, clockwise: Bool)

Appends an arc to the path.

func addCurve(to: CGPoint, controlPoint1: CGPoint, controlPoint2: CGPoint)

Appends a cubic Bézier curve to the path.

func addQuadCurve(to: CGPoint, controlPoint: CGPoint)

Appends a quadratic Bézier curve to the path.

func close()

Closes the most recent subpath.

func removeAllPoints()

Removes all points from the path, effectively deleting all subpaths.

func append(UIBezierPath)

Appends the contents of the specified path object to the path.

var cgPath: CGPath

The Core Graphics representation of the path.

var currentPoint: CGPoint

The current point in the graphics path.

