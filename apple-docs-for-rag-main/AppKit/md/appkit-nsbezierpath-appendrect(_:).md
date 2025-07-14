

- AppKit
- NSBezierPath
-  appendRect(\_:) 

Instance Method

# appendRect(\_:)

Appends a rectangular path to the path.

macOS

``` source
func appendRect(_ rect: NSRect)
```

## Parameters 

`rect`  

The rectangle describing the path to create.

## Discussion

Before adding the rectangle, this method moves the current point to the origin of the rectangle, which implicitly closes the current subpath (if any). The path is constructed by starting at the origin of `aRect` and adding line segments in a counterclockwise direction. The final segment is added using a close() message.

## See Also

### Related Documentation

class func fill(NSRect)

Fills the specified rectangular path with the current fill color.

class func stroke(NSRect)

Strokes the path of the specified rectangle using the current stroke color and the default drawing attributes.

init(rect: NSRect)

Creates and returns a new Bézier path object initialized with a rectangular path.

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

