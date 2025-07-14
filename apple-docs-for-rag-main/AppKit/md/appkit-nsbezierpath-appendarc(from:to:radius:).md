

- AppKit
- NSBezierPath
-  appendArc(from:to:radius:) 

Instance Method

# appendArc(from:to:radius:)

Appends an arc to the path.

macOS

``` source
func appendArc(
    from point1: NSPoint,
    to point2: NSPoint,
    radius: CGFloat
)
```

## Parameters 

`point1`  

The middle point of the angle.

`point2`  

The end point of the angle.

`radius`  

The radius of the circle inscribed in the angle.

## Discussion

The created arc is defined by a circle inscribed inside the angle specified by three points: the current point, the `fromPoint` parameter, and the `toPoint` parameter (in that order). The arc itself lies on the perimeter of the circle, whose radius is specified by the `radius` parameter. The arc is drawn between the two points of the circle that are tangent to the two legs of the angle.

The arc usually does not contain the points in the `fromPoint` and `toPoint` parameters. If the starting point of the arc does not coincide with the current point, a line is drawn between the two points. The starting point of the arc lies on the line defined by the current point and the `fromPoint` parameter.

You must set the path’s current point (using the move(to:) method or through the creation of a preceding line or curve segment) before you invoke this method. If the path is empty, this method raises an genericException exception.

Depending on the length of the arc, this method may add multiple connected curve segments to the path.

## See Also

### Appending Common Shapes to a Path

func append(NSBezierPath)

Appends the contents of the specified path object to the path.

func appendPoints(NSPointArray, count: Int)

Appends a series of line segments to the path.

func appendOval(in: NSRect)

Appends an oval path to the path, inscribing the oval in the specified rectangle.

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

