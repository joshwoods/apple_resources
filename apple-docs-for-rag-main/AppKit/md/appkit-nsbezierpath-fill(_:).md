

- AppKit
- NSBezierPath
-  fill(\_:) 

Type Method

# fill(\_:)

Fills the specified rectangular path with the current fill color.

macOS

``` source
class func fill(_ rect: NSRect)
```

## Parameters 

`rect`  

A rectangle in the current coordinate system.

## Discussion

This method fills the specified region immediately. This method uses the compositing operation returned by the `compositingOperation` method of `NSGraphicsContext`.

## See Also

### Related Documentation

func set()

Sets the color of subsequent drawing to the color that the color object represents.

init(rect: NSRect)

Creates and returns a new Bézier path object initialized with a rectangular path.

func appendRect(NSRect)

Appends a rectangular path to the path.

var compositingOperation: NSCompositingOperation

The graphics context’s global compositing operation setting.

### Drawing a Path

func stroke()

Draws a line along the path using the current stroke color and drawing attributes.

func fill()

Paints the region enclosed by the path.

class func stroke(NSRect)

Strokes the path of the specified rectangle using the current stroke color and the default drawing attributes.

class func strokeLine(from: NSPoint, to: NSPoint)

Strokes a line between two points using the current stroke color and the default drawing attributes.

class func drawPackedGlyphs(UnsafePointer&lt;CChar>, at: NSPoint)

Draws a set of packed glyphs at the specified point in the current coordinate system.

