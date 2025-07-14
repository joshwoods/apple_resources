

- AppKit
- NSImageRep
-  isOpaque 

Instance Property

# isOpaque

A Boolean value that indicates whether the image is opaque.

macOS

``` source
var isOpaque: Bool { get set }
```

## Discussion

The value of this property is true if the image should be treated as fully opaque; otherwise, false to indicate the image may include some transparent regions.

Use this property to test whether an image representation completely covers the area within the rectangle given by the size property.

The property value does not indicate whether the image has an alpha channel or if there is partial or complete transparency when drawing the image rep. Use the hasAlpha property to determine if the image has an alpha channel.

## See Also

### Specifying Information About the Representation

var bitsPerSample: Int

The number of bits per sample in the object (if the object is a planar image, this property contains the number of bits per sample per plane).

var colorSpaceName: NSColorSpaceName

The name of the color space used by the image data.

var hasAlpha: Bool

A Boolean value that indicates whether the image data has an alpha channel.

var pixelsHigh: Int

The height of the image, measured in pixels.

var pixelsWide: Int

The width of the image, measured in pixels.

var layoutDirection: NSImage.LayoutDirection

The layout direction for the image.

Device-Specific Value

A constant that is used by image representations to denote an attribute whose value changes to match the display device.

