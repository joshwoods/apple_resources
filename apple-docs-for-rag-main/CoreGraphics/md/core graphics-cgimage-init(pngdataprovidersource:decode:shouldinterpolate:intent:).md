

- Core Graphics
- CGImage
-  init(pngDataProviderSource:decode:shouldInterpolate:intent:) 

Initializer

# init(pngDataProviderSource:decode:shouldInterpolate:intent:)

Creates a bitmap image using PNG-encoded data supplied by a data provider.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(
    pngDataProviderSource source: CGDataProvider,
    decode: UnsafePointer?,
    shouldInterpolate: Bool,
    intent: CGColorRenderingIntent
)
```

## Parameters 

`source`  

A data provider supplying PNG-encoded data.

`decode`  

The decode array for the image. Typically a decode array is unnecessary, and you should pass `NULL`.

`shouldInterpolate`  

A Boolean value that specifies whether interpolation should occur. The interpolation setting specifies whether a pixel-smoothing algorithm should be applied to the image.

`intent`  

A CGColorRenderingIntent constant that specifies how to handle colors that are not located within the gamut of the destination color space of a graphics context.

## Return Value

A new CGImage. In Objective-C, you’re responsible for releasing this object by calling CGImageRelease.

## See Also

### Creating Images

init?(width: Int, height: Int, bitsPerComponent: Int, bitsPerPixel: Int, bytesPerRow: Int, space: CGColorSpace, bitmapInfo: CGBitmapInfo, provider: CGDataProvider, decode: UnsafePointer&lt;CGFloat>?, shouldInterpolate: Bool, intent: CGColorRenderingIntent)

Creates a bitmap image from data supplied by a data provider.

init?(jpegDataProviderSource: CGDataProvider, decode: UnsafePointer&lt;CGFloat>?, shouldInterpolate: Bool, intent: CGColorRenderingIntent)

Creates a bitmap image using JPEG-encoded data supplied by a data provider.

init?(headroom: Float, width: Int, height: Int, bitsPerComponent: Int, bitsPerPixel: Int, bytesPerRow: Int, space: CGColorSpace, bitmapInfo: CGBitmapInfo, provider: CGDataProvider, decode: UnsafePointer&lt;CGFloat>?, shouldInterpolate: Bool, intent: CGColorRenderingIntent)

