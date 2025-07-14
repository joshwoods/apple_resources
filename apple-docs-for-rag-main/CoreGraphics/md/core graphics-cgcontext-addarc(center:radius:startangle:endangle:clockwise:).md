

- Core Graphics
- CGContext
-  addArc(center:radius:startAngle:endAngle:clockwise:) 

Instance Method

# addArc(center:radius:startAngle:endAngle:clockwise:)

Adds an arc of a circle to the current path, specified with a radius and angles.

iOS 7.0+iPadOS 7.0+Mac CatalystmacOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addArc(
    center: CGPoint,
    radius: CGFloat,
    startAngle: CGFloat,
    endAngle: CGFloat,
    clockwise: Bool
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

## Discussion

This method calculates starting and ending points using the radius and angles you specify, uses a sequence of cubic Bézier curves to approximate a segment of a circle between those points, and then appends those curves to the current path.

The `clockwise` parameter determines the direction in which the arc is created; the actual direction of the final path is dependent on the current transformation matrix of the graphics context. In a flipped coordinate system (the default for UIView drawing methods in iOS), specifying a clockwise arc results in a counterclockwise arc after the transformation is applied.

If the current path already contains a subpath, this method adds a line connecting the current point to the starting point of the arc. If the current path is empty, his method creates a new subpath whose starting point is the starting point of the arc. The ending point of the arc becomes the new current point of the path.

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

func addArc(tangent1End: CGPoint, tangent2End: CGPoint, radius: CGFloat)

Adds an arc of a circle to the current path, specified with a radius and two tangent lines.

func addCurve(to: CGPoint, control1: CGPoint, control2: CGPoint)

Adds a cubic Bézier curve to the current path, with the specified end point and control points.

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

