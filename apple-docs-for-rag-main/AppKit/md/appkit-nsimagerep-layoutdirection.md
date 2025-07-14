

- AppKit
- NSImageRep
-  layoutDirection 

Instance Property

# layoutDirection

The layout direction for the image.

macOS 10.12+

``` source
var layoutDirection: NSImage.LayoutDirection { get set }
```

## Discussion

For possible values, see NSImage.LayoutDirection. The default value for new image representation objects is NSImage.LayoutDirection.unspecified.

## See Also

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

var pixelsWide: Int

The width of the image, measured in pixels.

Device-Specific Value

A constant that is used by image representations to denote an attribute whose value changes to match the display device.

