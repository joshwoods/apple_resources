

- Core Graphics
- CGContext
-  closePath() 

Instance Method

# closePath()

Closes and terminates the current path’s subpath.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func closePath()
```

## Discussion

Appends a line from the current point to the starting point of the current subpath and ends the subpath.

After closing the subpath, your application can begin a new subpath without first calling CGContextMoveToPoint. In this case, a new subpath is implicitly created with a starting and current point equal to the previous subpath’s starting point.

If the current path is empty or the current subpath is already closed, this function does nothing.

## See Also

### Constructing a Current Graphics Path

func beginPath()

Creates a new empty path in a graphics context.

func move(to: CGPoint)

Begins a new subpath at the specified point.

func addLine(to: CGPoint)

Appends a straight line segment from the current point to the specified point.

func addLines(between: [CGPoint])

Adds a sequence of connected straight-line segments to the current path.

func addRect(CGRect)

Adds a rectangular path to the current path.

func addRects([CGRect])

Adds a set of rectangular paths to the current path.

func addEllipse(in: CGRect)

Adds an ellipse that fits inside the specified rectangle.

func addArc(center: CGPoint, radius: CGFloat, startAngle: CGFloat, endAngle: CGFloat, clockwise: Bool)

Adds an arc of a circle to the current path, specified with a radius and angles.

func addArc(tangent1End: CGPoint, tangent2End: CGPoint, radius: CGFloat)

Adds an arc of a circle to the current path, specified with a radius and two tangent lines.

func addCurve(to: CGPoint, control1: CGPoint, control2: CGPoint)

Adds a cubic Bézier curve to the current path, with the specified end point and control points.

func addQuadCurve(to: CGPoint, control: CGPoint)

Adds a quadratic Bézier curve to the current path, with the specified end point and control point.

func addPath(CGPath)

Adds a previously created path object to the current path in a graphics context.

var path: CGPath?

Returns a path object built from the current path information in a graphics context.

func replacePathWithStrokedPath()

Replaces the path in the graphics context with the stroked version of the path.

