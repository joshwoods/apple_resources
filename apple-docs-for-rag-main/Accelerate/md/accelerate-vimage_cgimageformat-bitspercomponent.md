

- Accelerate
- vImage_CGImageFormat
-  bitsPerComponent 

Instance Property

# bitsPerComponent

The number of bits that represents one channel of data in one pixel.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var bitsPerComponent: UInt32
```

## Discussion

For ARGB8888, this is 8. Expected values are 1, 2, 4, 5, 8, 10, 12, 16, or 32.

## See Also

### Instance properties

var bitsPerPixel: UInt32

The number of bits that represents one pixel.

var colorSpace: Unmanaged&lt;CGColorSpace>!

A description of the position of the pixel data in the image, relative to a reference XYZ color space.

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

