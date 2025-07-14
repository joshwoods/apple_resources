

- Accelerate
- vImage_CGImageFormat
-  colorSpace 

Instance Property

# colorSpace

A description of the position of the pixel data in the image, relative to a reference XYZ color space.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var colorSpace: Unmanaged!
```

## See Also

### Instance properties

var bitsPerComponent: UInt32

The number of bits that represents one channel of data in one pixel.

var bitsPerPixel: UInt32

The number of bits that represents one pixel.

var bitmapInfo: CGBitmapInfo

The component information that describes the color channels.

var version: UInt32

The version number.

var decode: UnsafePointer&lt;CGFloat>!

The decode array for the image.

var renderingIntent: CGColorRenderingIntent

A rendering intent constant that specifies how Core Graphics handles colors that aren’t within the destination color space gamut.

var componentCount: Int

The number of color and alpha channels.

