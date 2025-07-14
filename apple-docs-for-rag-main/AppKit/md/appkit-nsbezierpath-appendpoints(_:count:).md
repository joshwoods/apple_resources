

- AppKit
- NSBezierPath
-  appendPoints(\_:count:) 

Instance Method

# appendPoints(\_:count:)

Appends a series of line segments to the path.

macOS

``` source
func appendPoints(
    _ points: NSPointArray,
    count: Int
)
```

## Parameters 

`points`  

A C-style array of `NSPoint` data types, each of which contains the end point of the next line segment.

`count`  

The number of points in the `points` parameter.

## Discussion

This method interprets the points as a set of connected line segments. If the current path contains an open subpath, a line is created from the last point in that subpath to the first point in the points array. If the current path is empty, the first point in the points array is used to set the starting point of the line segments. Subsequent line segments are added using the remaining points in the array.

This method does not close the path that is created. If you wish to create a closed path, you must do so by explicitly invoking the receiver’s close() method.

## See Also

### Appending Common Shapes to a Path

func append(NSBezierPath)

Appends the contents of the specified path object to the path.

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

