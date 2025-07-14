

- MetalKit
- MTKView
-  multisampleColorTexture 

Instance Property

# multisampleColorTexture

The multisample color sample texture to render into.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var multisampleColorTexture: (any MTLTexture)? { get }
```

## Discussion

The format of this texture is determined by the value of the colorPixelFormat and sampleCount properties.

The default value is `nil`. This value is also `nil` if the specified pixel format is MTLPixelFormat.invalid, or if sampleCount is less than or equal to 1.

## See Also

### Retrieving Render Target Information

var currentRenderPassDescriptor: MTLRenderPassDescriptor?

A render pass descriptor to draw into the current drawable.

var currentDrawable: (any CAMetalDrawable)?

The drawable to use for the current frame.

var depthStencilTexture: (any MTLTexture)?

A packed depth and stencil texture associated with the current drawable object’s texture.

var depthStencilStorageMode: MTLStorageMode

The storage mode that the packed depth and stencil texture use.

