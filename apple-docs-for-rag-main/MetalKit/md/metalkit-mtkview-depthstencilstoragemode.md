

- MetalKit
- MTKView
-  depthStencilStorageMode 

Instance Property

# depthStencilStorageMode

The storage mode that the packed depth and stencil texture use.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
var depthStencilStorageMode: MTLStorageMode { get set }
```

## Discussion

The default value is MTLStorageMode.private.

## See Also

### Retrieving Render Target Information

var currentRenderPassDescriptor: MTLRenderPassDescriptor?

A render pass descriptor to draw into the current drawable.

var currentDrawable: (any CAMetalDrawable)?

The drawable to use for the current frame.

var depthStencilTexture: (any MTLTexture)?

A packed depth and stencil texture associated with the current drawable object’s texture.

var multisampleColorTexture: (any MTLTexture)?

The multisample color sample texture to render into.

