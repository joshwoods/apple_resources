

- SwiftUI
-  Path 

Structure

# Path

The outline of a 2D shape.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct Path
```

## Topics

### Creating a path

init()

Creates an empty path.

init(_:)

Creates an empty path, then executes a closure to add its initial elements.

init(ellipseIn: CGRect)

Creates a path as an ellipse within the given rectangle.

init(roundedRect: CGRect, cornerRadius: CGFloat, style: RoundedCornerStyle)

Creates a path containing a rounded rectangle.

init(roundedRect: CGRect, cornerSize: CGSize, style: RoundedCornerStyle)

Creates a path containing a rounded rectangle.

init(roundedRect: CGRect, cornerRadii: RectangleCornerRadii, style: RoundedCornerStyle)

Creates a path as the given rounded rectangle, which may have uneven corner radii.

### Getting the path’s characteristics

var boundingRect: CGRect

A rectangle containing all path segments.

var cgPath: CGPath

An immutable path representing the elements in the path.

func contains(CGPoint, eoFill: Bool) -> Bool

Returns true if the path contains a specified point.

var currentPoint: CGPoint?

Returns the last point in the path, or nil if the path contains no points.

var description: String

A description of the path that may be used to recreate the path via `init?(_:)`.

var isEmpty: Bool

A Boolean value indicating whether the path contains zero elements.

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

func closeSubpath()

Closes and completes the current subpath.

### Transforming the path

func applying(CGAffineTransform) -> Path

Returns a path constructed by applying the transform to all points of the path.

func offsetBy(dx: CGFloat, dy: CGFloat) -> Path

Returns a path constructed by translating all its points.

func trimmedPath(from: CGFloat, to: CGFloat) -> Path

Returns a partial copy of the path.

### Performing operations on the path

func addRoundedRect(in: CGRect, cornerSize: CGSize, style: RoundedCornerStyle, transform: CGAffineTransform)

Adds a rounded rectangle to the path.

func intersection(Path, eoFill: Bool) -> Path

Returns a new path with filled regions common to both paths.

func lineIntersection(Path, eoFill: Bool) -> Path

Returns a new path with a line from this path that overlaps the filled regions of the given path.

func lineSubtraction(Path, eoFill: Bool) -> Path

Returns a new path with a line from this path that does not overlap the filled region of the given path.

func normalized(eoFill: Bool) -> Path

Returns a new weakly-simple copy of this path.

func subtracting(Path, eoFill: Bool) -> Path

Returns a new path with filled regions from this path that are not in the given path.

func symmetricDifference(Path, eoFill: Bool) -> Path

Returns a new path with filled regions either from this path or the given path, but not in both.

func union(Path, eoFill: Bool) -> Path

Returns a new path with filled regions in either this path or the given path.

### Operating over path elements

func forEach((Path.Element) -> Void)

Calls `body` with each element in the path.

enum Element

An element of a path.

### Applying a style

func strokedPath(StrokeStyle) -> Path

Returns a stroked copy of the path using `style` to define how the stroked outline is created.

### Instance Methods

func addRoundedRect(in: CGRect, cornerRadii: RectangleCornerRadii, style: RoundedCornerStyle, transform: CGAffineTransform)

Adds a rounded rectangle with uneven corners to the path.

## Relationships

### Conforms To

- Animatable
- Copyable
- CustomStringConvertible
- Equatable
- LosslessStringConvertible
- Sendable
- Shape
- View

