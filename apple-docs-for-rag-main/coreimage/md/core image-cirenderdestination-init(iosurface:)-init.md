

- Core Image
- CIRenderDestination
-  init(ioSurface:) 

Initializer

# init(ioSurface:)

Creates a render destination based on an IOSurface object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
init(ioSurface surface: IOSurface)
```

## Parameters 

`surface`  

The IOSurface render target.

## Return Value

A CIRenderDestination object for rendering to an IOSurface object.

## Discussion

The destination's colorSpace property will default to a CGColorSpace created by querying the IOSurface object's attributes.

## See Also

### Creating a Render Destination

init(pixelBuffer: CVPixelBuffer)

Creates a render destination based on a Core Video pixel buffer.

init(mtlTexture: any MTLTexture, commandBuffer: (any MTLCommandBuffer)?)

Creates a render destination based on a Metal texture.

init(width: Int, height: Int, pixelFormat: MTLPixelFormat, commandBuffer: (any MTLCommandBuffer)?, mtlTextureProvider: (() -> any MTLTexture)?)

Creates a render destination based on a Metal texture with specified pixel format.

init(glTexture: UInt32, target: UInt32, width: Int, height: Int)

Creates a render destination based on an OpenGL texture.

init(bitmapData: UnsafeMutableRawPointer, width: Int, height: Int, bytesPerRow: Int, format: CIFormat)

Creates a render destination based on a client-managed buffer.

