

- Core Image
- CIRenderDestination
-  init(width:height:pixelFormat:commandBuffer:mtlTextureProvider:) 

Initializer

# init(width:height:pixelFormat:commandBuffer:mtlTextureProvider:)

Creates a render destination based on a Metal texture with specified pixel format.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
init(
    width: Int,
    height: Int,
    pixelFormat: MTLPixelFormat,
    commandBuffer: (any MTLCommandBuffer)?,
    mtlTextureProvider block: (() -> any MTLTexture)? = nil
)
```

## Parameters 

`width`  

Width of the MTLTexture that will be returned by block.

`height`  

Height of the MTLTexture that will be returned by block.

`pixelFormat`  

Pixel format of the MTLTexture that will be returned by block.

`commandBuffer`  

An optional MTLCommandBuffer used for rendering to the MTLTexture.

`block`  

MTLTexture-rendering provider block to be called lazily when the destination is rendered to. The block must return a texture of MTLTextureType of MTLTextureType.type2D.

## Return Value

A CIRenderDestination object for rendering to a Metal texture.

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

init(glTexture: UInt32, target: UInt32, width: Int, height: Int)

Creates a render destination based on an OpenGL texture.

init(bitmapData: UnsafeMutableRawPointer, width: Int, height: Int, bytesPerRow: Int, format: CIFormat)

Creates a render destination based on a client-managed buffer.

