

- Core Image
- CIRenderDestination
-  init(bitmapData:width:height:bytesPerRow:format:) 

Initializer

# init(bitmapData:width:height:bytesPerRow:format:)

Creates a render destination based on a client-managed buffer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
init(
    bitmapData data: UnsafeMutableRawPointer,
    width: Int,
    height: Int,
    bytesPerRow: Int,
    format: CIFormat
)
```

## Parameters 

`data`  

Pointer to raw bits of a client-managed buffer that is at least (`bytesPerRow` \* `height`) bytes in size.

`width`  

Width of the bitmap image in pixels.

`height`  

Height of the bitmap image in pixels.

`bytesPerRow`  

Number of bytes per row of data.

`format`  

Color format specifying how the colors are laid out in memory (for example, RGBA8).

## Return Value

A CIRenderDestination object for rendering to a client-managed buffer.

## Discussion

The destination's colorSpace property will default to a CGColorSpace created with sRGB, extendedSRGB, or genericGrayGamma2_2.

## See Also

### Creating a Render Destination

init(pixelBuffer: CVPixelBuffer)

Creates a render destination based on a Core Video pixel buffer.

init(ioSurface: IOSurface)

Creates a render destination based on an IOSurface object.

init(mtlTexture: any MTLTexture, commandBuffer: (any MTLCommandBuffer)?)

Creates a render destination based on a Metal texture.

init(width: Int, height: Int, pixelFormat: MTLPixelFormat, commandBuffer: (any MTLCommandBuffer)?, mtlTextureProvider: (() -> any MTLTexture)?)

Creates a render destination based on a Metal texture with specified pixel format.

init(glTexture: UInt32, target: UInt32, width: Int, height: Int)

Creates a render destination based on an OpenGL texture.

