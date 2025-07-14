

- UIKit
- UIBezierPath
-  append(\_:) 

Instance Method

# append(\_:)

Appends the contents of the specified path object to the path.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func append(_ bezierPath: UIBezierPath)
```

## Parameters 

`bezierPath`  

The path to add to the receiver.

## Discussion

This method adds the commands used to create the path in `bezierPath` to the end of the receiver’s path. This method does not explicitly try to connect the subpaths in the two objects, although the operations in `bezierPath` might still cause that effect.

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

var cgPath: CGPath

The Core Graphics representation of the path.

var currentPoint: CGPoint

The current point in the graphics path.

