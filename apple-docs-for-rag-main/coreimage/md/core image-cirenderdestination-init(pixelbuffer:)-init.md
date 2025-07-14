

- Core Image
- CIRenderDestination
-  init(pixelBuffer:) 

Initializer

# init(pixelBuffer:)

Creates a render destination based on a Core Video pixel buffer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
init(pixelBuffer: CVPixelBuffer)
```

## Parameters 

`pixelBuffer`  

The CVPixelBuffer render target.

## Return Value

A CIRenderDestination object for rendering to a CVPixelBuffer.

## Discussion

The destination's colorSpace property will default to a CGColorSpace created by querying the CVPixelBuffer object's attributes.

## See Also

### Creating a Render Destination

init(ioSurface: IOSurface)

Creates a render destination based on an IOSurface object.

init(mtlTexture: any MTLTexture, commandBuffer: (any MTLCommandBuffer)?)

Creates a render destination based on a Metal texture.

init(width: Int, height: Int, pixelFormat: MTLPixelFormat, commandBuffer: (any MTLCommandBuffer)?, mtlTextureProvider: (() -> any MTLTexture)?)

Creates a render destination based on a Metal texture with specified pixel format.

init(glTexture: UInt32, target: UInt32, width: Int, height: Int)

Creates a render destination based on an OpenGL texture.

init(bitmapData: UnsafeMutableRawPointer, width: Int, height: Int, bytesPerRow: Int, format: CIFormat)

Creates a render destination based on a client-managed buffer.

