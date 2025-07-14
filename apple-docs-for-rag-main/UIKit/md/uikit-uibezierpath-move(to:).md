

- UIKit
- UIBezierPath
-  move(to:) 

Instance Method

# move(to:)

Moves the path’s current point to the specified location.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func move(to point: CGPoint)
```

## Parameters 

`point`  

A point in the current coordinate system.

## Discussion

This method implicitly ends the current subpath (if any) and sets the current point to the value in the `point` parameter. When ending the previous subpath, this method does not actually close the subpath. Therefore, the first and last points of the previous subpath are not connected to each other.

For many path operations, you must call this method before issuing any commands that cause a line or curve segment to be drawn.

## See Also

### Constructing a path

func addLine(to: CGPoint)

Appends a straight line to the path.

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

