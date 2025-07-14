

- UIKit
- UIBezierPath
-  addCurve(to:controlPoint1:controlPoint2:) 

Instance Method

# addCurve(to:controlPoint1:controlPoint2:)

Appends a cubic Bézier curve to the path.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func addCurve(
    to endPoint: CGPoint,
    controlPoint1: CGPoint,
    controlPoint2: CGPoint
)
```

## Parameters 

`endPoint`  

The end point of the curve.

`controlPoint1`  

The first control point to use when computing the curve.

`controlPoint2`  

The second control point to use when computing the curve.

## Discussion

This method appends a cubic Bézier curve from the current point to the end point specified by the `endPoint` parameter. The two control points define the curvature of the segment. The following image shows an approximation of a cubic Bézier curve given a set of initial points. The exact curvature of the segment involves a complex mathematical relationship between all of the points and is well documented online.

You must set the path’s current point (using the move(to:) method or through the previous creation of a line or curve segment) before you call this method. If the path is empty, this method does nothing. After adding the curve segment, this method updates the current point to the value in `point`.

## See Also

### Constructing a path

func move(to: CGPoint)

Moves the path’s current point to the specified location.

func addLine(to: CGPoint)

Appends a straight line to the path.

func addArc(withCenter: CGPoint, radius: CGFloat, startAngle: CGFloat, endAngle: CGFloat, clockwise: Bool)

Appends an arc to the path.

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

