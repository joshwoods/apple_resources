

- Core Image
- CIRenderDestination
-  init(mtlTexture:commandBuffer:) 

Initializer

# init(mtlTexture:commandBuffer:)

Creates a render destination based on a Metal texture.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
init(
    mtlTexture texture: any MTLTexture,
    commandBuffer: (any MTLCommandBuffer)?
)
```

## Parameters 

`texture`  

The MTLTexture object for rendering with MTLTextureType of MTLTextureType.type2D.

`commandBuffer`  

An optional MTLCommandBuffer to use for rendering to the MTLTexture destination.

## Return Value

A CIRenderDestination object for rendering to a Metal buffer.

## Discussion

Rendering to a MTLTexture-backed CIRenderDestination is supported by only MTLTexture-backed CIContext objects. The texture must have MTLTextureType of MTLTextureType.type2D.

The destination's colorSpace property will default to a CGColorSpace created with sRGB, extendedSRGB, or genericGrayGamma2_2.

## See Also

### Creating a Render Destination

init(pixelBuffer: CVPixelBuffer)

Creates a render destination based on a Core Video pixel buffer.

init(ioSurface: IOSurface)

Creates a render destination based on an IOSurface object.

init(width: Int, height: Int, pixelFormat: MTLPixelFormat, commandBuffer: (any MTLCommandBuffer)?, mtlTextureProvider: (() -> any MTLTexture)?)

Creates a render destination based on a Metal texture with specified pixel format.

init(glTexture: UInt32, target: UInt32, width: Int, height: Int)

Creates a render destination based on an OpenGL texture.

init(bitmapData: UnsafeMutableRawPointer, width: Int, height: Int, bytesPerRow: Int, format: CIFormat)

Creates a render destination based on a client-managed buffer.

