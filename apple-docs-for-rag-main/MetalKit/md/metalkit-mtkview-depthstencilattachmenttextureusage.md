

- MetalKit
- MTKView
-  depthStencilAttachmentTextureUsage 

Instance Property

# depthStencilAttachmentTextureUsage

The texture usage characteristics that the view uses when creating the depth and stencil textures.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var depthStencilAttachmentTextureUsage: MTLTextureUsage { get set }
```

## Discussion

The default value is renderTarget.

## See Also

### Configuring the Render Target Properties

var depthStencilPixelFormat: MTLPixelFormat

The format used to generate the depthStencilTexture object.

var clearDepth: Double

The depth value to use to clear the depth target when creating a render pass descriptor.

var clearStencil: UInt32

The stencil value to use to clear the stencil target when creating a render pass descriptor.

