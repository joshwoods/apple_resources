

- AppKit
- NSBezierPath
-  strokeLine(from:to:) 

Type Method

# strokeLine(from:to:)

Strokes a line between two points using the current stroke color and the default drawing attributes.

macOS

``` source
class func strokeLine(
    from point1: NSPoint,
    to point2: NSPoint
)
```

## Parameters 

`point1`  

The starting point of the line.

`point2`  

The ending point of the line.

## Discussion

This method strokes the specified path immediately.

## See Also

### Related Documentation

func move(to: NSPoint)

Moves the path’s current point to the specified location.

func line(to: NSPoint)

Appends a straight line to the path.

### Drawing a Path

func stroke()

Draws a line along the path using the current stroke color and drawing attributes.

func fill()

Paints the region enclosed by the path.

class func fill(NSRect)

Fills the specified rectangular path with the current fill color.

class func stroke(NSRect)

Strokes the path of the specified rectangle using the current stroke color and the default drawing attributes.

class func drawPackedGlyphs(UnsafePointer&lt;CChar>, at: NSPoint)

Draws a set of packed glyphs at the specified point in the current coordinate system.

