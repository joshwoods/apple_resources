

- SwiftUI
- Path
-  closeSubpath() 

Instance Method

# closeSubpath()

Closes and completes the current subpath.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func closeSubpath()
```

## Discussion

Appends a line from the current point to the starting point of the current subpath and ends the subpath.

After closing the subpath, your application can begin a new subpath without first calling `move(to:)`. In this case, a new subpath is implicitly created with a starting and current point equal to the previous subpath’s starting point.

## See Also

### Drawing a path

func move(to: CGPoint)

Begins a new subpath at the specified point.

func addArc(center: CGPoint, radius: CGFloat, startAngle: Angle, endAngle: Angle, clockwise: Bool, transform: CGAffineTransform)

Adds an arc of a circle to the path, specified with a radius and angles.

func addArc(tangent1End: CGPoint, tangent2End: CGPoint, radius: CGFloat, transform: CGAffineTransform)

Adds an arc of a circle to the path, specified with a radius and two tangent lines.

func addCurve(to: CGPoint, control1: CGPoint, control2: CGPoint)

Adds a cubic Bézier curve to the path, with the specified end point and control points.

func addEllipse(in: CGRect, transform: CGAffineTransform)

Adds an ellipse that fits inside the specified rectangle to the path.

func addLine(to: CGPoint)

Appends a straight line segment from the current point to the specified point.

func addLines([CGPoint])

Adds a sequence of connected straight-line segments to the path.

func addPath(Path, transform: CGAffineTransform)

Appends another path value to this path.

func addQuadCurve(to: CGPoint, control: CGPoint)

Adds a quadratic Bézier curve to the path, with the specified end point and control point.

func addRect(CGRect, transform: CGAffineTransform)

Adds a rectangular subpath to the path.

func addRects([CGRect], transform: CGAffineTransform)

Adds a set of rectangular subpaths to the path.

func addRelativeArc(center: CGPoint, radius: CGFloat, startAngle: Angle, delta: Angle, transform: CGAffineTransform)

Adds an arc of a circle to the path, specified with a radius and a difference in angle.

func addRoundedRect(in: CGRect, cornerSize: CGSize, style: RoundedCornerStyle, transform: CGAffineTransform)

Adds a rounded rectangle to the path.

