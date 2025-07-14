

- AppKit
- NSImageRep
-  bitsPerSample 

Instance Property

# bitsPerSample

The number of bits per sample in the object (if the object is a planar image, this property contains the number of bits per sample per plane).

macOS

``` source
var bitsPerSample: Int { get set }
```

## Discussion

The number of bits used to specify each component of data in a single pixel (for example, a value of 8 for an RGBA image means that each pixel is comprised of four 8-bit values) or NSImageRepMatchesDevice.

A subclass can set this property when loading image data to notify the parent class of how many bits each sample uses. Specifying a value that differs from the actual image data does not change the bit depth of the image.

## See Also

### Related Documentation

var bitsPerPixel: Int

The number of bits allocated for each pixel in each plane of data.

var samplesPerPixel: Int

The number of components for each pixel.

var isPlanar: Bool

A Boolean value that indicates whether the image data is in a planar configuration.

### Specifying Information About the Representation

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

var layoutDirection: NSImage.LayoutDirection

The layout direction for the image.

Device-Specific Value

A constant that is used by image representations to denote an attribute whose value changes to match the display device.

