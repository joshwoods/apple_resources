

- AppKit
- NSImageRep
-  size 

Instance Property

# size

The size of the image representation, measured in points in the user coordinate space.

macOS

``` source
var size: NSSize { get set }
```

## Discussion

This size is the size of the image representation when it’s rendered. It is not necessarily the same as the width and height of the image in pixels as specified by the image data, nor must it be equal to the size set for the `NSImage` object that wraps this image representation.

The size of an image representation combined with the physical dimensions of the image data determine the resolution of the image.

## See Also

### Related Documentation

var pixelsHigh: Int

The height of the image, measured in pixels.

var pixelsWide: Int

The width of the image, measured in pixels.

func draw() -> Bool

Implemented by subclasses to draw the image in the current coordinate system.

