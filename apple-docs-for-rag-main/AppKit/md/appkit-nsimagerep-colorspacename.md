

- AppKit
- NSImageRep
-  colorSpaceName 

Instance Property

# colorSpaceName

The name of the color space used by the image data.

macOS

``` source
var colorSpaceName: NSColorSpaceName { get set }
```

## Discussion

By default, an `NSImageRep` object’s color space name is `NSCalibratedRGBColorSpace`. Color space names are defined as part of the `NSColor` class, in `NSGraphics.h`. The following are valid color space names:

- `NSCalibratedWhiteColorSpace`

- `NSCalibratedBlackColorSpace`

- `NSCalibratedRGBColorSpace`

- `NSDeviceWhiteColorSpace`

- `NSDeviceBlackColorSpace`

- `NSDeviceRGBColorSpace`

- `NSDeviceCMYKColorSpace`

- `NSNamedColorSpace`

- `NSCustomColorSpace`

## See Also

### Specifying Information About the Representation

var bitsPerSample: Int

The number of bits per sample in the object (if the object is a planar image, this property contains the number of bits per sample per plane).

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

