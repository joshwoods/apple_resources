

- AppKit
- NSImageRep
-  pixelsWide 

Instance Property

# pixelsWide

The width of the image, measured in pixels.

macOS

``` source
var pixelsWide: Int { get set }
```

## Discussion

The value of this property is the width of the image, measured in the units of the device coordinate space. This value is usually derived from the image data itself.

Subclasses can use this property when loading image data to notify the parent class of the image width. Setting this property does not change the actual number of pixels in the image.

## See Also

### Related Documentation

var NSImageRepMatchesDevice: Int

A constant indicating that the value of certain attributes, such as the number of colors or bits per sample, will change to match the display device.

var size: NSSize

The size of the image representation, measured in points in the user coordinate space.

### Specifying Information About the Representation

var bitsPerSample: Int

The number of bits per sample in the object (if the object is a planar image, this property contains the number of bits per sample per plane).

var colorSpaceName: NSColorSpaceName

The name of the color space used by the image data.

var hasAlpha: Bool

A Boolean value that indicates whether the image data has an alpha channel.

var isOpaque: Bool

A Boolean value that indicates whether the image is opaque.

var pixelsHigh: Int

The height of the image, measured in pixels.

var layoutDirection: NSImage.LayoutDirection

The layout direction for the image.

Device-Specific Value

A constant that is used by image representations to denote an attribute whose value changes to match the display device.

