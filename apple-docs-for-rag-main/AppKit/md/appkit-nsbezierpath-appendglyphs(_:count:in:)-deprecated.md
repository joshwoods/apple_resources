

- AppKit
- NSBezierPath
-  appendGlyphs(\_:count:in:) Deprecated

Instance Method

# appendGlyphs(\_:count:in:)

Appends the outlines of the specified glyphs to the path.

macOS 10.0–10.14Deprecated

``` source
func appendGlyphs(
    _ glyphs: UnsafeMutablePointer,
    count: Int,
    in font: NSFont
)
```

Deprecated

Use append(withCGGlyphs:count:in:) instead.

## Parameters 

`glyphs`  

A C-style array of `NSGlyph` data types to add to the path.

`count`  

The number of glyphs in the `glyphs` parameter.

`font`  

The font in which the glyphs are encoded.

## Discussion

If the glyphs are not encoded in the font specified by the `fontObj` parameter—that is, the font does not have an entry for one of the specified glyphs—then no path is appended to the receiver.

You must set the path’s current point (using the move(to:) method or through the creation of a preceding line or curve segment) before you invoke this method. If the path is empty, this method raises an genericException exception.

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

func appendPackedGlyphs(UnsafePointer&lt;CChar>)

Appends an array of packed glyphs to the path.

Deprecated

