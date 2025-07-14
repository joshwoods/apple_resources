

- AppKit
-  NSBezierPath 

Class

# NSBezierPath

An object that can create paths using PostScript-style commands.

macOS

``` source
class NSBezierPath
```

## Overview

Paths consist of straight and curved line segments joined together. Paths can form recognizable shapes such as rectangles, ovals, arcs, and glyphs; they can also form complex polygons using either straight or curved line segments. A single path can be closed by connecting its two endpoints, or it can be left open.

An NSBezierPath object can contain multiple disconnected paths, whether they are closed or open. Each of these paths is referred to as a subpath. The subpaths of a Bézier path object must be manipulated as a group. The only way to manipulate subpaths individually is to create separate NSBezierPath objects for each.

For a given NSBezierPath object, you can stroke the path’s outline or fill the region occupied by the path. You can also use the path as a clipping region for views or other regions. Using methods of NSBezierPath, you can also perform hit detection on the filled or stroked path. Hit detection is needed to implement interactive graphics, as in rubber banding and dragging operations.

The current graphics context is automatically saved and restored for all drawing operations involving Bézier path objects, so your application does not need to worry about the graphics settings changing across invocations.

## Topics

### Creating a Bézier Path

init(ovalIn: NSRect)

Creates and returns a new Bézier path object initialized with an oval path inscribed in the specified rectangle.

init(rect: NSRect)

Creates and returns a new Bézier path object initialized with a rectangular path.

init(roundedRect: NSRect, xRadius: CGFloat, yRadius: CGFloat)

Creates and returns a new Bézier path object initialized with a rounded rectangular path.

init(cgPath: CGPath)

var flattened: NSBezierPath

A flattened version of the path object.

var reversed: NSBezierPath

A path containing the reversed contents of the current path object.

### Constructing a Path

func move(to: NSPoint)

Moves the path’s current point to the specified location.

func line(to: NSPoint)

Appends a straight line to the path.

func curve(to: NSPoint, controlPoint1: NSPoint, controlPoint2: NSPoint)

Adds a Bezier cubic curve to the path.

func curve(to: NSPoint, controlPoint: NSPoint)

func close()

Closes the most recently added subpath.

func relativeMove(to: NSPoint)

Moves the path’s current point to a new point whose location is the specified distance from the current point.

func relativeLine(to: NSPoint)

Appends a straight line segment to the path starting at the current point and moving towards the specified point, relative to the current location.

func relativeCurve(to: NSPoint, controlPoint1: NSPoint, controlPoint2: NSPoint)

Adds a Bezier cubic curve to the path from the current point to a new location, which is specified as a relative distance from the current point.

func relativeCurve(to: NSPoint, controlPoint: NSPoint)

### Appending Common Shapes to a Path

func append(NSBezierPath)

Appends the contents of the specified path object to the path.

func appendPoints(NSPointArray, count: Int)

Appends a series of line segments to the path.

func appendOval(in: NSRect)

Appends an oval path to the path, inscribing the oval in the specified rectangle.

func appendArc(from: NSPoint, to: NSPoint, radius: CGFloat)

Appends an arc to the path.

func appendArc(withCenter: NSPoint, radius: CGFloat, startAngle: CGFloat, endAngle: CGFloat)

Appends an arc of a circle to the path.

func appendArc(withCenter: NSPoint, radius: CGFloat, startAngle: CGFloat, endAngle: CGFloat, clockwise: Bool)

Appends an arc of a circle to the path.

func appendRect(NSRect)

Appends a rectangular path to the path.

func appendRoundedRect(NSRect, xRadius: CGFloat, yRadius: CGFloat)

Appends a rounded rectangular path to the path.

func append(withCGGlyph: CGGlyph, in: NSFont)

Appends an outline of the specified glyph to the path.

func append(withCGGlyphs: UnsafePointer&lt;CGGlyph>, count: Int, in: NSFont)

Appends the outlines of the specified glyphs to the path.

func appendGlyph(NSGlyph, in: NSFont)

Appends an outline of the specified glyph to the path.

Deprecated

func appendGlyphs(UnsafeMutablePointer&lt;NSGlyph>, count: Int, in: NSFont)

Appends the outlines of the specified glyphs to the path.

Deprecated

func appendPackedGlyphs(UnsafePointer&lt;CChar>)

Appends an array of packed glyphs to the path.

Deprecated

### Accessing a Path’s Attributes

var windingRule: NSBezierPath.WindingRule

The winding rule used to fill the path.

var lineCapStyle: NSBezierPath.LineCapStyle

The line cap style for the path.

var lineJoinStyle: NSBezierPath.LineJoinStyle

The line join style for the path.

var lineWidth: CGFloat

The width of stroked path lines.

var miterLimit: CGFloat

The limit at which miter joins are converted to bevel joins.

var flatness: CGFloat

The accuracy with which curves are rendered.

func getLineDash(UnsafeMutablePointer&lt;CGFloat>?, count: UnsafeMutablePointer&lt;Int>?, phase: UnsafeMutablePointer&lt;CGFloat>?)

Returns the line-stroking pattern for the receiver.

func setLineDash(UnsafePointer&lt;CGFloat>?, count: Int, phase: CGFloat)

Sets the line-stroking pattern for the path.

### Configuring Default Path Attributes

class var defaultWindingRule: NSBezierPath.WindingRule

Returns the default winding rule used to fill all paths.

class var defaultLineCapStyle: NSBezierPath.LineCapStyle

Returns the default line cap style for all paths.

class var defaultLineJoinStyle: NSBezierPath.LineJoinStyle

Returns the default line join style for all paths.

class var defaultLineWidth: CGFloat

Returns the default line width for the all paths.

class var defaultMiterLimit: CGFloat

Returns the default miter limit for all paths.

class var defaultFlatness: CGFloat

The default flatness value for all paths.

### Drawing a Path

func stroke()

Draws a line along the path using the current stroke color and drawing attributes.

func fill()

Paints the region enclosed by the path.

class func fill(NSRect)

Fills the specified rectangular path with the current fill color.

class func stroke(NSRect)

Strokes the path of the specified rectangle using the current stroke color and the default drawing attributes.

class func strokeLine(from: NSPoint, to: NSPoint)

Strokes a line between two points using the current stroke color and the default drawing attributes.

class func drawPackedGlyphs(UnsafePointer&lt;CChar>, at: NSPoint)

Draws a set of packed glyphs at the specified point in the current coordinate system.

### Specifying a Clipping Path

func addClip()

Intersects the area enclosed by the path with the clipping path of the current graphics context and makes the resulting shape the current clipping path.

func setClip()

Replaces the clipping path of the current graphics context with the area inside the path.

class func clip(NSRect)

Intersects the specified rectangle with the clipping path of the current graphics context and makes the resulting shape the current clipping path.

### Performing Hit-Testing

func contains(NSPoint) -> Bool

Returns a Boolean value that indicates whether the path contains the specified point.

### Querying a Path

var bounds: NSRect

The bounding box of the path.

var controlPointBounds: NSRect

The bounding box of the path, including any control points.

var currentPoint: NSPoint

The current point (the trailing point or ending point in the most recently added segment).

var isEmpty: Bool

A Boolean value that indicates whether the path is empty.

### Applying Transformations

func transform(using: AffineTransform)

Transforms all points in the path using the specified transform.

### Accessing Elements of a Path

var cgPath: CGPath

var elementCount: Int

The total number of path elements in the path.

func element(at: Int) -> NSBezierPath.ElementType

Returns the type of path element at the specified index.

func element(at: Int, associatedPoints: NSPointArray?) -> NSBezierPath.ElementType

Gets the element type and (and optionally) the associated points for the path element at the specified index.

func removeAllPoints()

Removes all path elements from the path, effectively clearing the path.

func setAssociatedPoints(NSPointArray?, at: Int)

Changes the points associated with the specified path element.

### Constants

enum ElementType

Constants that specify basic path element commands.

enum LineJoinStyle

Constants that specify the shape of the joins between connected segments of a stroked path.

enum LineCapStyle

Constants that specify the shape of endpoints for an open path when it is stroked.

enum WindingRule

Constants that specify the winding rule a Bézier path uses.

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

### Shapes and Paths

Convenience Functions

Draw rectangles and other primitive shapes using these convenience functions.

