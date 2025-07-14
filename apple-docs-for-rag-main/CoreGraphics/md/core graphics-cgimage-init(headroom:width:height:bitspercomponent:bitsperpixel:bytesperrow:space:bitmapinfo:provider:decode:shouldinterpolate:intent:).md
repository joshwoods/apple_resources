

- Core Graphics
- CGImage
-  init(headroom:width:height:bitsPerComponent:bitsPerPixel:bytesPerRow:space:bitmapInfo:provider:decode:shouldInterpolate:intent:) 

Initializer

# init(headroom:width:height:bitsPerComponent:bitsPerPixel:bytesPerRow:space:bitmapInfo:provider:decode:shouldInterpolate:intent:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init?(
    headroom: Float,
    width: Int,
    height: Int,
    bitsPerComponent: Int,
    bitsPerPixel: Int,
    bytesPerRow: Int,
    space: CGColorSpace,
    bitmapInfo: CGBitmapInfo,
    provider: CGDataProvider,
    decode: UnsafePointer?,
    shouldInterpolate: Bool,
    intent: CGColorRenderingIntent
)
```

## See Also

### Creating Images

init?(width: Int, height: Int, bitsPerComponent: Int, bitsPerPixel: Int, bytesPerRow: Int, space: CGColorSpace, bitmapInfo: CGBitmapInfo, provider: CGDataProvider, decode: UnsafePointer&lt;CGFloat>?, shouldInterpolate: Bool, intent: CGColorRenderingIntent)

Creates a bitmap image from data supplied by a data provider.

init?(jpegDataProviderSource: CGDataProvider, decode: UnsafePointer&lt;CGFloat>?, shouldInterpolate: Bool, intent: CGColorRenderingIntent)

Creates a bitmap image using JPEG-encoded data supplied by a data provider.

init?(pngDataProviderSource: CGDataProvider, decode: UnsafePointer&lt;CGFloat>?, shouldInterpolate: Bool, intent: CGColorRenderingIntent)

Creates a bitmap image using PNG-encoded data supplied by a data provider.

