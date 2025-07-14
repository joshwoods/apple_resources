

- Accelerate
- vImage_CGImageFormat
-  init(bitsPerComponent:bitsPerPixel:colorSpace:bitmapInfo:version:decode:renderingIntent:) 

Initializer

# init(bitsPerComponent:bitsPerPixel:colorSpace:bitmapInfo:version:decode:renderingIntent:)

Creates a Core Graphics image format.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    bitsPerComponent: UInt32,
    bitsPerPixel: UInt32,
    colorSpace: Unmanaged!,
    bitmapInfo: CGBitmapInfo,
    version: UInt32,
    decode: UnsafePointer!,
    renderingIntent: CGColorRenderingIntent
)
```

## Parameters 

`bitsPerComponent`  

The number of bits that represents one channel of data in one pixel.

`bitsPerPixel`  

The number of bits that represents one pixel.

`colorSpace`  

A description of the position of the pixel data in the image, relative to a reference XYZ color space.

`bitmapInfo`  

The component information that describes the color channels.

`version`  

Reserved for future expansion — pass `0` here.

`decode`  

The decode array for the image. See decode for more information.

`renderingIntent`  

A rendering intent constant that specifies how Core Graphics handles colors that aren’t within the destination color space gamut.

## See Also

### Initializers

init?(bitsPerComponent: Int, bitsPerPixel: Int, colorSpace: CGColorSpace, bitmapInfo: CGBitmapInfo, renderingIntent: CGColorRenderingIntent)

Creates a Core Graphics image format with a color space instance and default decode array.

init?(cgImage: CGImage)

Creates a Core Graphics image format of the specified image.

init()

Creates an empty Core Graphics image format.

