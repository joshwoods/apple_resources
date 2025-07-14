

- Core Graphics
-  CGMutablePath 

Class

# CGMutablePath

A mutable graphics path: a mathematical description of shapes or lines to be drawn in a graphics context.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CGMutablePath
```

## Overview

Neither `CGPath` nor CGMutablePath define functions to draw a path. To draw a Core Graphics path to a graphics context, you add the path to the graphics context by calling addPath(_:) and then call one of the context’s drawing functions—see CGContext.

Each figure in the graphics path is constructed with a connected set of lines and Bézier curves, called a *subpath*. A subpath has an ordered set of *path elements* that represent single steps in the construction of the subpath. (For example, a line segment from one corner of a rectangle to another corner is a path element. Every subpath includes a *starting point*, which is the first point in the subpath. The path also maintains a *current point*, which is the last point in the last subpath.

To append a new subpath onto a mutable path, your application typically calls CGPathMoveToPoint to set the subpath’s starting point and initial current point, followed by a series of “add” calls (such as CGPathAddLineToPoint) to add line segments and curves to the subpath. As segments or curves are added to the subpath, the subpath’s current point is updated to point to the end of the last segment or curve to be added. The lines and curves of a subpath are always connected, but they are not required to form a closed set of lines. Your application explicitly closes a subpath by calling closeSubpath(). Closing the subpath adds a line segment that terminates at the subpath’s starting point, and also changes how those lines are rendered—for more information see Paths in Quartz 2D Programming Guide.

## Topics

### Creating Graphics Paths

init()

Creates a mutable graphics path.

### Copying a Graphics Path

func mutableCopy() -> CGMutablePath?

Creates a mutable copy of an existing graphics path.

func mutableCopy(using: UnsafePointer&lt;CGAffineTransform>?) -> CGMutablePath?

Creates a mutable copy of a graphics path transformed by a transformation matrix.

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

## Relationships

### Inherits From

- CGPath

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Quartz 2D Programming Guide

### 2D Drawing

class CGContext

A Quartz 2D drawing environment.

class CGImage

A bitmap image or image mask.

class CGPath

An immutable graphics path: a mathematical description of shapes or lines to be drawn in a graphics context.

class CGLayer

An offscreen context for reusing content drawn with Core Graphics.

