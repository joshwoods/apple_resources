

- AppKit
- NSImageRep
-  hasAlpha 

Instance Property

# hasAlpha

A Boolean value that indicates whether the image data has an alpha channel.

macOS

``` source
var hasAlpha: Bool { get set }
```

## Discussion

The value of this property is true if the receiver has a known alpha channel; otherwise, false.

Subclasses can set this property when loading image data to notify the parent class whether that data contains an alpha component. Specifying a value of true does not add an alpha channel to the image data itself; it merely records the fact that the data has an alpha channel.

## See Also

### Specifying Information About the Representation

var bitsPerSample: Int

The number of bits per sample in the object (if the object is a planar image, this property contains the number of bits per sample per plane).

var colorSpaceName: NSColorSpaceName

The name of the color space used by the image data.

var isOpaque: Bool

A Boolean value that indicates whether the image is opaque.

var pixelsHigh: Int

The height of the image, measured in pixels.

var pixelsWide: Int

The width of the image, measured in pixels.

var layoutDirection: NSImage.LayoutDirection

The layout direction for the image.

Device-Specific Value

A constant that is used by image representations to denote an attribute whose value changes to match the display device.

