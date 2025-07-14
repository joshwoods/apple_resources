

- Core Graphics
- CGContext
-  init(data:width:height:bitsPerComponent:bytesPerRow:space:bitmapInfo:) 

Initializer

# init(data:width:height:bitsPerComponent:bytesPerRow:space:bitmapInfo:)

Creates a bitmap graphics context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(
    data: UnsafeMutableRawPointer?,
    width: Int,
    height: Int,
    bitsPerComponent: Int,
    bytesPerRow: Int,
    space: CGColorSpace,
    bitmapInfo: UInt32
)
```

## Parameters 

`data`  

A pointer to the destination in memory where the drawing is to be rendered. The size of this memory block should be at least `(bytesPerRow*height)` bytes.

Pass `nil` if you want this function to allocate memory for the bitmap. This frees you from managing your own memory, which reduces memory leak issues.

`width`  

The width, in pixels, of the required bitmap.

`height`  

The height, in pixels, of the required bitmap.

`bitsPerComponent`  

The number of bits to use for each component of a pixel in memory. For example, for a 32-bit pixel format and an RGB color space, you would specify a value of 8 bits per component. For the list of supported pixel formats, see “Supported Pixel Formats” in the Graphics Contexts chapter of Quartz 2D Programming Guide.

`bytesPerRow`  

The number of bytes of memory to use per row of the bitmap. If the `data` parameter is `NULL`, passing a value of `0` causes the value to be calculated automatically.

`space`  

The color space to use for the bitmap context. Note that indexed color spaces are not supported for bitmap graphics contexts.

`bitmapInfo`  

Constants that specify whether the bitmap should contain an alpha channel, the alpha channel’s relative location in a pixel, and information about whether the pixel components are floating-point or integer values. The constants for specifying the alpha channel information are declared with the CGImageAlphaInfo type but can be passed to this parameter safely. You can also pass the other constants associated with the CGBitmapInfo type.

For an example of how to specify the color space, bits per pixel, bits per pixel component, and bitmap information, see Graphics Contexts.

## Return Value

A new bitmap context, or `nil` if a context could not be created. In Objective-C, you’re responsible for releasing this object using CGContextRelease.

## Discussion

When you draw into this context, Core Graphics renders your drawing as bitmapped data in the specified block of memory.

The pixel format for a new bitmap context is determined by three parameters—the number of bits per component, the color space, and an alpha option (expressed as a CGBitmapInfo constant). The alpha value determines the opacity of a pixel when it is drawn.

## See Also

### Creating Bitmap Graphics Contexts

init?(data: UnsafeMutableRawPointer?, width: Int, height: Int, bitsPerComponent: Int, bytesPerRow: Int, space: CGColorSpace, bitmapInfo: UInt32, releaseCallback: CGBitmapContextReleaseDataCallback?, releaseInfo: UnsafeMutableRawPointer?)

Creates a bitmap graphics context with the specified callback function.

typealias CGBitmapContextReleaseDataCallback

A callback function used to release data associate with the bitmap context.

