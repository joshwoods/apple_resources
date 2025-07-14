

- AppKit
- NSBezierPath
-  fill() 

Instance Method

# fill()

Paints the region enclosed by the path.

macOS

``` source
func fill()
```

## Discussion

This method fills the path using the current fill color and the receiver’s current winding rule. If the path contains any open subpaths, this method implicitly closes them before painting the fill region.

The painted region includes the pixels right up to, but not including, the path line itself. For paths with large line widths, this can result in overlap between the fill region and the stroked path (which is itself centered on the path line).

## See Also

### Related Documentation

func set()

Sets the color of subsequent drawing to the color that the color object represents.

var windingRule: NSBezierPath.WindingRule

The winding rule used to fill the path.

### Drawing a Path

func stroke()

Draws a line along the path using the current stroke color and drawing attributes.

class func fill(NSRect)

Fills the specified rectangular path with the current fill color.

class func stroke(NSRect)

Strokes the path of the specified rectangle using the current stroke color and the default drawing attributes.

class func strokeLine(from: NSPoint, to: NSPoint)

Strokes a line between two points using the current stroke color and the default drawing attributes.

class func drawPackedGlyphs(UnsafePointer&lt;CChar>, at: NSPoint)

Draws a set of packed glyphs at the specified point in the current coordinate system.

