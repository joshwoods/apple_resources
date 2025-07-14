

- Accelerate
- vImage_CGImageFormat
-  init(cgImage:) 

Initializer

# init(cgImage:)

Creates a Core Graphics image format of the specified image.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
init?(cgImage: CGImage)
```

## Parameters 

`cgImage`  

The source Core Graphics image.

## Mentioned in 

Converting bitmap data between Core Graphics images and vImage buffers

## See Also

### Initializers

init(bitsPerComponent: UInt32, bitsPerPixel: UInt32, colorSpace: Unmanaged&lt;CGColorSpace>!, bitmapInfo: CGBitmapInfo, version: UInt32, decode: UnsafePointer&lt;CGFloat>!, renderingIntent: CGColorRenderingIntent)

Creates a Core Graphics image format.

init?(bitsPerComponent: Int, bitsPerPixel: Int, colorSpace: CGColorSpace, bitmapInfo: CGBitmapInfo, renderingIntent: CGColorRenderingIntent)

Creates a Core Graphics image format with a color space instance and default decode array.

init()

Creates an empty Core Graphics image format.

