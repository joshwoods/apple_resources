

- UIKit
-  UIBezierPath 

Class

# UIBezierPath

A path that consists of straight and curved line segments that you can render in your custom views.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class UIBezierPath
```

## Overview

You use this class initially to specify just the geometry for your path. Paths can define simple shapes such as rectangles, ovals, and arcs or they can define complex polygons that incorporate a mixture of straight and curved line segments. After defining the shape, you can use additional methods of this class to render the path in the current drawing context.

A UIBezierPath object combines the geometry of a path with attributes that describe the path during rendering. You set the geometry and attributes separately and can change them independent of one another. After you have the object configured the way you want it, you can tell it to draw itself in the current context. Because the creation, configuration, and rendering process are all distinct steps, Bézier path objects can be reused easily in your code. You can even use the same object to render the same shape multiple times, perhaps changing the rendering options between successive drawing calls.

You set the geometry of a path by manipulating the path’s current point. When you create a new empty path object, the current point is undefined and must be set explicitly. To move the current point without drawing a segment, you use the move(to:) method. All other methods result in the addition of either a line or curve segments to the path. The methods for adding new segments always assume you are starting at the current point and ending at some new point that you specify. After adding the segment, the end point of the new segment automatically becomes the current point.

A single Bézier path object can contain any number of open or closed subpaths, where each subpath represents a connected series of path segments. Calling the close() method closes a subpath by adding a straight line segment from the current point to the first point in the subpath. Calling the move(to:) method ends the current subpath (without closing it) and sets the starting point of the next subpath. The subpaths of a Bézier path object share the same drawing attributes and must be manipulated as a group. To draw subpaths with different attributes, you must put each subpath in its own UIBezierPath object.

After configuring the geometry and attributes of a Bézier path, you draw the path in the current graphics context using the stroke() and fill() methods. The stroke() method traces the outline of the path using the current stroke color and the attributes of the Bézier path object. Similarly, the fill() method fills in the area enclosed by the path using the current fill color. (You set the stroke and fill color using the UIColor class.)

In addition to using a Bézier path object to draw shapes, you can also use it to define a new clipping region. The addClip() method intersects the shape represented by the path object with the current clipping region of the graphics context. During subsequent drawing, only content that lies within the new intersection region is actually rendered to the graphics context.

## Topics

### Creating a Bézier path

convenience init(rect: CGRect)

Creates and returns a new Bézier path object with a rectangular path.

convenience init(ovalIn: CGRect)

Creates and returns a new Bézier path object with an inscribed oval path in the specified rectangle.

convenience init(roundedRect: CGRect, cornerRadius: CGFloat)

Creates and returns a new Bézier path object with a rounded rectangular path.

convenience init(roundedRect: CGRect, byRoundingCorners: UIRectCorner, cornerRadii: CGSize)

Creates and returns a new Bézier path object with a rectangular path rounded at the specified corners.

convenience init(arcCenter: CGPoint, radius: CGFloat, startAngle: CGFloat, endAngle: CGFloat, clockwise: Bool)

Creates and returns a new Bézier path object with an arc of a circle.

convenience init(cgPath: CGPath)

Creates and returns a new Bézier path object with the contents of a Core Graphics path.

func reversing() -> UIBezierPath

Creates and returns a new Bézier path object with the reversed contents of the current path.

init()

Creates and returns an empty path object.

init?(coder: NSCoder)

Creates a Bézier path object from data in an unarchiver.

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

var cgPath: CGPath

The Core Graphics representation of the path.

var currentPoint: CGPoint

The current point in the graphics path.

### Accessing drawing properties

var lineWidth: CGFloat

The line width of the path.

var lineCapStyle: CGLineCap

The shape of the endpoints of a stroked path.

var lineJoinStyle: CGLineJoin

The shape of the joints between connected segments of a stroked path.

var miterLimit: CGFloat

The limiting value that helps avoid spikes at junctions between connected line segments.

var flatness: CGFloat

The factor that determines the rendering accuracy for curved path segments.

var usesEvenOddFillRule: Bool

A Boolean value that indicates whether the even-odd winding rule is in use for drawing paths.

func setLineDash(UnsafePointer&lt;CGFloat>?, count: Int, phase: CGFloat)

Sets the line-stroking pattern for the path.

func getLineDash(UnsafeMutablePointer&lt;CGFloat>?, count: UnsafeMutablePointer&lt;Int>?, phase: UnsafeMutablePointer&lt;CGFloat>?)

Retrieves the line-stroking pattern for the path.

### Drawing paths

func fill()

Uses the current drawing properties to paint the region that the path encloses.

func fill(with: CGBlendMode, alpha: CGFloat)

Uses the specified blend mode and transparency values to paint the region that the path encloses.

func stroke()

Draws a line along the path using the current drawing properties.

func stroke(with: CGBlendMode, alpha: CGFloat)

Draws a line along the path using the specified blend mode and transparency values.

### Specifying clipping paths

func addClip()

Uses the clipping path of the current graphics context to intersect the region that the path encloses, and makes the resulting shape the current clipping path.

### Performing hit-testing

func contains(CGPoint) -> Bool

Returns a Boolean value that indicates whether the specified point is within the region that the path encloses.

var isEmpty: Bool

A Boolean value that indicates whether the path has any valid elements.

var bounds: CGRect

The bounding rectangle of the path.

### Applying transformations

func apply(CGAffineTransform)

Transforms all points in the path using the specified affine transform matrix.

### Constants

struct UIRectCorner

The corners of a rectangle.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Paths

func UIRectFill(CGRect)

Fills the specified rectangle with the current color.

func UIRectFillUsingBlendMode(CGRect, CGBlendMode)

Fills a rectangle with the current fill color using the specified blend mode.

func UIRectFrame(CGRect)

Draws a frame around the inside of the specified rectangle.

func UIRectFrameUsingBlendMode(CGRect, CGBlendMode)

Draws a frame around the inside of a rectangle using the specified blend mode.

