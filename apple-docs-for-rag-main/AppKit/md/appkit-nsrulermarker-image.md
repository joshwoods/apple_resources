

- AppKit
- NSRulerMarker
-  image 

Instance Property

# image

The receiver’s image.

macOS

``` source
var image: NSImage { get set }
```

## Discussion

The image used to draw the marker must be appropriate for the orientation of the ruler. Markers may need to look different on a horizontal ruler than on a vertical ruler, and the ruler view neither scales nor rotates the images.

## See Also

### Setting the image

var imageOrigin: NSPoint

The point in the receiver’s image that is positioned at the receiver’s location on the ruler view.

var imageRectInRuler: NSRect

The rectangle occupied by the receiver’s image.

var thicknessRequiredInRuler: CGFloat

The amount of the receiver’s image that’s displayed above or to the left of the ruler view’s baseline.

