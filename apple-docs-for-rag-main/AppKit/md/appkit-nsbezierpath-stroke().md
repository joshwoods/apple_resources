

- AppKit
- NSBezierPath
-  stroke() 

Instance Method

# stroke()

Draws a line along the path using the current stroke color and drawing attributes.

macOS

``` source
func stroke()
```

## Discussion

The drawn line is centered on the path with its sides parallel to the path segment. This method uses the current drawing attributes associated with the receiver. If a particular attribute is not set for the receiver, this method uses the corresponding default attribute.

## See Also

### Related Documentation

func set()

Sets the color of subsequent drawing to the color that the color object represents.

### Drawing a Path

func fill()

Paints the region enclosed by the path.

class func fill(NSRect)

Fills the specified rectangular path with the current fill color.

class func stroke(NSRect)

Strokes the path of the specified rectangle using the current stroke color and the default drawing attributes.

class func strokeLine(from: NSPoint, to: NSPoint)

Strokes a line between two points using the current stroke color and the default drawing attributes.

class func drawPackedGlyphs(UnsafePointer&lt;CChar>, at: NSPoint)

Draws a set of packed glyphs at the specified point in the current coordinate system.

