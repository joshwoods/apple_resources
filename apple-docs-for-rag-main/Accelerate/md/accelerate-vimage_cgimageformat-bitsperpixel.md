

- Accelerate
- vImage_CGImageFormat
-  bitsPerPixel 

Instance Property

# bitsPerPixel

The number of bits that represents one pixel.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var bitsPerPixel: UInt32
```

## Discussion

For ARGB8888, this is 32.

The number of color components derives from the color space, and the number of alpha components (zero or one) derives from the bitmapInfo.

## See Also

### Instance properties

var bitsPerComponent: UInt32

The number of bits that represents one channel of data in one pixel.

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

