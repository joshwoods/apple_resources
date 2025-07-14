

- Accelerate
- vImage_CGImageFormat
-  init(bitsPerComponent:bitsPerPixel:colorSpace:bitmapInfo:renderingIntent:) 

Initializer

# init(bitsPerComponent:bitsPerPixel:colorSpace:bitmapInfo:renderingIntent:)

Creates a Core Graphics image format with a color space instance and default decode array.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
init?(
    bitsPerComponent: Int,
    bitsPerPixel: Int,
    colorSpace: CGColorSpace,
    bitmapInfo: CGBitmapInfo,
    renderingIntent: CGColorRenderingIntent = .defaultIntent
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

`renderingIntent`  

A rendering intent constant that specifies how Core Graphics handles colors that aren’t within the destination color space gamut.

## See Also

### Initializers

init(bitsPerComponent: UInt32, bitsPerPixel: UInt32, colorSpace: Unmanaged&lt;CGColorSpace>!, bitmapInfo: CGBitmapInfo, version: UInt32, decode: UnsafePointer&lt;CGFloat>!, renderingIntent: CGColorRenderingIntent)

Creates a Core Graphics image format.

init?(cgImage: CGImage)

Creates a Core Graphics image format of the specified image.

init()

Creates an empty Core Graphics image format.

