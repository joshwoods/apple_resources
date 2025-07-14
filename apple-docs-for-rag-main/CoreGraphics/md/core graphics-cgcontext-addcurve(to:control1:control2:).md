

- Core Graphics
- CGContext
-  addCurve(to:control1:control2:) 

Instance Method

# addCurve(to:control1:control2:)

Adds a cubic Bézier curve to the current path, with the specified end point and control points.

iOS 7.0+iPadOS 7.0+Mac CatalystmacOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addCurve(
    to end: CGPoint,
    control1: CGPoint,
    control2: CGPoint
)
```

## Parameters 

`end`  

The point, in user space coordinates, at which to end the curve.

`control1`  

The first control point of the curve, in user space coordinates.

`control2`  

The second control point of the curve, in user space coordinates.

## Discussion

This method constructs a curve starting from the path’s current point and ending at the specified end point, with curvature defined by the two control points. After this method appends that curve to the current path, the end point of the curve becomes the path’s current point.

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

func addQuadCurve(to: CGPoint, control: CGPoint)

Adds a quadratic Bézier curve to the current path, with the specified end point and control point.

func addPath(CGPath)

Adds a previously created path object to the current path in a graphics context.

func closePath()

Closes and terminates the current path’s subpath.

var path: CGPath?

Returns a path object built from the current path information in a graphics context.

func replacePathWithStrokedPath()

Replaces the path in the graphics context with the stroked version of the path.

