

- AppKit
- NSBezierPath
-  appendRoundedRect(\_:xRadius:yRadius:) 

Instance Method

# appendRoundedRect(\_:xRadius:yRadius:)

Appends a rounded rectangular path to the path.

macOS 10.5+

``` source
func appendRoundedRect(
    _ rect: NSRect,
    xRadius: CGFloat,
    yRadius: CGFloat
)
```

## Parameters 

`rect`  

The rectangle that defines the basic shape of the path.

`xRadius`  

The radius of each corner oval along the x-axis. Values larger than half the rectangle’s width are clamped to half the width.

`yRadius`  

The radius of each corner oval along the y-axis. Values larger than half the rectangle’s height are clamped to half the height.

## Discussion

The path is constructed in a counter-clockwise direction, starting at the top-left corner of the rectangle. If either one of the radius parameters contains the value `0.0`, the returned path is a plain rectangle without rounded corners.

## See Also

### Related Documentation

init(roundedRect: NSRect, xRadius: CGFloat, yRadius: CGFloat)

Creates and returns a new Bézier path object initialized with a rounded rectangular path.

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

