

- MetalKit
- MTKView
-  depthStencilTexture 

Instance Property

# depthStencilTexture

A packed depth and stencil texture associated with the current drawable object’s texture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var depthStencilTexture: (any MTLTexture)? { get }
```

## Discussion

The value of depthStencilPixelFormat determines the format of this texture.

The default value is `nil`. This value is also `nil` if the specified pixel format is MTLPixelFormat.invalid.

## See Also

### Retrieving Render Target Information

var currentRenderPassDescriptor: MTLRenderPassDescriptor?

A render pass descriptor to draw into the current drawable.

var currentDrawable: (any CAMetalDrawable)?

The drawable to use for the current frame.

var depthStencilStorageMode: MTLStorageMode

The storage mode that the packed depth and stencil texture use.

var multisampleColorTexture: (any MTLTexture)?

The multisample color sample texture to render into.

