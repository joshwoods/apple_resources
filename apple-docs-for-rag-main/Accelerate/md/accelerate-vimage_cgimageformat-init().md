

- Accelerate
- vImage_CGImageFormat
-  init() 

Initializer

# init()

Creates an empty Core Graphics image format.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init()
```

## See Also

### Initializers

init(bitsPerComponent: UInt32, bitsPerPixel: UInt32, colorSpace: Unmanaged&lt;CGColorSpace>!, bitmapInfo: CGBitmapInfo, version: UInt32, decode: UnsafePointer&lt;CGFloat>!, renderingIntent: CGColorRenderingIntent)

Creates a Core Graphics image format.

init?(bitsPerComponent: Int, bitsPerPixel: Int, colorSpace: CGColorSpace, bitmapInfo: CGBitmapInfo, renderingIntent: CGColorRenderingIntent)

Creates a Core Graphics image format with a color space instance and default decode array.

init?(cgImage: CGImage)

Creates a Core Graphics image format of the specified image.

