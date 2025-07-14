

- AppKit
- NSBezierPath
-  appendPackedGlyphs(\_:) Deprecated

Instance Method

# appendPackedGlyphs(\_:)

Appends an array of packed glyphs to the path.

macOS 10.0–10.14Deprecated

``` source
func appendPackedGlyphs(_ packedGlyphs: UnsafePointer)
```

Deprecated

Use append(withCGGlyphs:count:in:) instead.

## Parameters 

`packedGlyphs`  

A C-style array containing one or more `CGGlyph` data types terminated by a `NULL` character.

## Discussion

You should avoid using this method directly. Instead, use the appendGlyph(_:in:) and appendGlyphs(_:count:in:) methods to append glyphs to a path.

## See Also

### Related Documentation

class func drawPackedGlyphs(UnsafePointer&lt;CChar>, at: NSPoint)

Draws a set of packed glyphs at the specified point in the current coordinate system.

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

