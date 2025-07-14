

- AppKit
- NSBezierPath
-  appendArc(withCenter:radius:startAngle:endAngle:) 

Instance Method

# appendArc(withCenter:radius:startAngle:endAngle:)

Appends an arc of a circle to the path.

macOS

``` source
func appendArc(
    withCenter center: NSPoint,
    radius: CGFloat,
    startAngle: CGFloat,
    endAngle: CGFloat
)
```

## Parameters 

`center`  

Specifies the center point of the circle used to define the arc.

`radius`  

Specifies the radius of the circle used to define the arc.

`startAngle`  

Specifies the starting angle of the arc, measured in degrees counterclockwise from the x-axis.

`endAngle`  

Specifies the end angle of the arc, measured in degrees counterclockwise from the x-axis.

## Discussion

The created arc lies on the perimeter of the circle, between the angles specified by the `startAngle` and `endAngle` parameters. The arc is drawn in a counterclockwise direction. If the receiver’s path is empty, this method sets the current point to the beginning of the arc before adding the arc segment. If the receiver’s path is not empty, a line is drawn from the current point to the starting point of the arc.

Depending on the length of the arc, this method may add multiple connected curve segments to the path.

## See Also

### Appending Common Shapes to a Path

func append(NSBezierPath)

Appends the contents of the specified path object to the path.

func appendPoints(NSPointArray, count: Int)

Appends a series of line segments to the path.

func appendOval(in: NSRect)

Appends an oval path to the path, inscribing the oval in the specified rectangle.

func appendArc(from: NSPoint, to: NSPoint, radius: CGFloat)

Appends an arc to the path.

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

