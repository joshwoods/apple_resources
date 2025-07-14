

- Core Image
- CIRenderDestination
-  init(glTexture:target:width:height:) 

Initializer

# init(glTexture:target:width:height:)

Creates a render destination based on an OpenGL texture.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
init(
    glTexture texture: UInt32,
    target: UInt32,
    width: Int,
    height: Int
)
```

## Parameters 

`texture`  

`GLTexture`-backed texture data.

`target`  

A value denoting the type of destination. Use `GL_TEXTURE_2D `if your texture dimensions are a power of two, or `GL_TEXTURE_RECTANGLE_EXT` otherwise.

`width`  

Width of the texture in texels.

`height`  

Height of the texture in texels.

## Return Value

A CIRenderDestination object for rendering to a `GLTexture` supported by `GLContext`-backed CIContext.

## Discussion

Rendering to a `GLTexture`-backed CIRenderDestination is supported by only `GLContext`-backed CIContext.

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

init(bitmapData: UnsafeMutableRawPointer, width: Int, height: Int, bytesPerRow: Int, format: CIFormat)

Creates a render destination based on a client-managed buffer.

