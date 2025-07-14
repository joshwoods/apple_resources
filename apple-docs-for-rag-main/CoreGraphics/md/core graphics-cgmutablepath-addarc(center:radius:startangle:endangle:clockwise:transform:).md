

- Core Graphics
- CGMutablePath
-  addArc(center:radius:startAngle:endAngle:clockwise:transform:) 

Instance Method

# addArc(center:radius:startAngle:endAngle:clockwise:transform:)

Adds an arc of a circle to the path, specified with a radius and angles.

iOS 7.0+iPadOS 7.0+Mac CatalystmacOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addArc(
    center: CGPoint,
    radius: CGFloat,
    startAngle: CGFloat,
    endAngle: CGFloat,
    clockwise: Bool,
    transform: CGAffineTransform = .identity
)
```

## Parameters 

`center`  

The center of the arc, in user space coordinates.

`radius`  

The radius of the arc, in user space coordinates.

`startAngle`  

The angle to the starting point of the arc, measured in radians from the positive x-axis.

`endAngle`  

The angle to the end point of the arc, measured in radians from the positive x-axis.

`clockwise`  

true to make a clockwise arc; false to make a counterclockwise arc.

`transform`  

An affine transform to apply to the arc before adding to the path. Defaults to the identity transform if not specified.

## Discussion

This method calculates starting and ending points using the radius and angles you specify, uses a sequence of cubic Bézier curves to approximate a segment of a circle between those points, and then appends those curves to the path.

The `clockwise` parameter determines the direction in which the arc is created; the actual direction of the final path is dependent on the `transform` parameter and the current transform of a context where the path is drawn. In a flipped coordinate system (the default for UIView drawing methods in iOS), specifying a clockwise arc results in a counterclockwise arc after the transformation is applied.

If the path already contains a subpath, this method adds a line connecting the current point to the starting point of the arc. If the current path is empty, this method creates a new subpath whose starting point is the starting point of the arc. The ending point of the arc becomes the new current point of the path.

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

func addRects([CGRect], transform: CGAffineTransform)

Adds a set of rectangular subpaths to the path.

func addEllipse(in: CGRect, transform: CGAffineTransform)

Adds an ellipse that fits inside the specified rectangle.

func addRoundedRect(in: CGRect, cornerWidth: CGFloat, cornerHeight: CGFloat, transform: CGAffineTransform)

Adds a subpath to the path, in the shape of a rectangle with rounded corners.

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

