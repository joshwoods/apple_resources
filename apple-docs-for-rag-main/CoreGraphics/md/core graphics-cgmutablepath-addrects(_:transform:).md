

- Core Graphics
- CGMutablePath
-  addRects(\_:transform:) 

Instance Method

# addRects(\_:transform:)

Adds a set of rectangular subpaths to the path.

iOS 7.0+iPadOS 7.0+Mac CatalystmacOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addRects(
    _ rects: [CGRect],
    transform: CGAffineTransform = .identity
)
```

## Parameters 

`rects`  

An array of rectangles, specified in user space coordinates.

`transform`  

An affine transform to apply to the rectangles before adding to the path. Defaults to the identity transform if not specified.

## Discussion

Calling this convenience method is equivalent to repeatedly calling the addRect(_:transform:) method for each rectangle in the array.

## See Also

### Constructing a Graphics Path

func move(to: CGPoint, transform: CGAffineTransform)

Begins a new subpath at the specified point.

func addLine(to: CGPoint, transform: CGAffineTransform)

Appends a straight line segment from the current point to the specified point.

func addLines(between: [CGPoint], transform: CGAffineTransform)

Adds a sequence of connected straight-line segments to the path.

func addRect(CGRect, transform: CGAffineTransform)

Adds a rectangular subpath to the path.

func addEllipse(in: CGRect, transform: CGAffineTransform)

Adds an ellipse that fits inside the specified rectangle.

func addRoundedRect(in: CGRect, cornerWidth: CGFloat, cornerHeight: CGFloat, transform: CGAffineTransform)

Adds a subpath to the path, in the shape of a rectangle with rounded corners.

func addArc(center: CGPoint, radius: CGFloat, startAngle: CGFloat, endAngle: CGFloat, clockwise: Bool, transform: CGAffineTransform)

Adds an arc of a circle to the path, specified with a radius and angles.

func addArc(tangent1End: CGPoint, tangent2End: CGPoint, radius: CGFloat, transform: CGAffineTransform)

Adds an arc of a circle to the path, specified with a radius and two tangent lines.

func addRelativeArc(center: CGPoint, radius: CGFloat, startAngle: CGFloat, delta: CGFloat, transform: CGAffineTransform)

Adds an arc of a circle to the path, specified with a radius and a difference in angle.

func addCurve(to: CGPoint, control1: CGPoint, control2: CGPoint, transform: CGAffineTransform)

Adds a cubic Bézier curve to the path, with the specified end point and control points.

func addQuadCurve(to: CGPoint, control: CGPoint, transform: CGAffineTransform)

Adds a quadratic Bézier curve to the path, with the specified end point and control point.

func addPath(CGPath, transform: CGAffineTransform)

Appends another path object to the path.

func closeSubpath()

Closes and completes a subpath in a mutable graphics path.

