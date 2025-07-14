

- AppKit
- NSBezierPath
-  drawPackedGlyphs(\_:at:) 

Type Method

# drawPackedGlyphs(\_:at:)

Draws a set of packed glyphs at the specified point in the current coordinate system.

macOS

``` source
class func drawPackedGlyphs(
    _ packedGlyphs: UnsafePointer,
    at point: NSPoint
)
```

## Parameters 

`packedGlyphs`  

A C-style array containing one or more `CGGlyph` data types terminated by a `NULL` character.

`point`  

The starting point at which to draw the glyphs.

## Discussion

This method draws the glyphs immediately.

You should avoid using this method directly. Instead, use the appendGlyph(_:in:) and appendGlyphs(_:count:in:) methods to create a path with one or more glyphs.

## See Also

### Related Documentation

func appendPackedGlyphs(UnsafePointer&lt;CChar>)

Appends an array of packed glyphs to the path.

Deprecated

func set()

Sets the color of subsequent drawing to the color that the color object represents.

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

