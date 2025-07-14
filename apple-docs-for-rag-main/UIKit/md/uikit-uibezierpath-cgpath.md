

- UIKit
- UIBezierPath
-  cgPath 

Instance Property

# cgPath

The Core Graphics representation of the path.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var cgPath: CGPath { get set }
```

## Discussion

This property contains a snapshot of the path at any given point in time. Getting this property returns an immutable path object that you can pass to Core Graphics functions. The path object itself is owned by the `UIBezierPath` object and is valid only until you make further modifications to the path.

You can set the value of this property to a path you built using the functions of the Core Graphics framework. When setting a new path, this method makes a copy of the path you provide.

## See Also

### Constructing a path

func move(to: CGPoint)

Moves the path’s current point to the specified location.

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

var currentPoint: CGPoint

The current point in the graphics path.

