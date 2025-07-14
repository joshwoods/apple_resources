

- AppKit
- NSRulerMarker
-  imageRectInRuler 

Instance Property

# imageRectInRuler

The rectangle occupied by the receiver’s image.

macOS

``` source
var imageRectInRuler: NSRect { get }
```

## Discussion

The rectangle occupied by the receiver’s image, in the ruler view’s coordinate system, accounting for whether the ruler view’s coordinate system is flipped.

## See Also

### Related Documentation

func draw(NSRect)

Draws the receiver’s image that appears in the supplied rectangle.

### Setting the image

var image: NSImage

The receiver’s image.

var imageOrigin: NSPoint

The point in the receiver’s image that is positioned at the receiver’s location on the ruler view.

var thicknessRequiredInRuler: CGFloat

The amount of the receiver’s image that’s displayed above or to the left of the ruler view’s baseline.

