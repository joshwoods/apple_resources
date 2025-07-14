

- MetalKit
- MTKView
-  clearStencil 

Instance Property

# clearStencil

The stencil value to use to clear the stencil target when creating a render pass descriptor.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var clearStencil: UInt32 { get set }
```

## Discussion

If you specified that you want a stencil texture, the view configures any render passes to use the stencil texture, with a load action of MTLLoadAction.clear and the value of this property as the value to clear it to. The default value is `0`.

## See Also

### Configuring the Render Target Properties

var depthStencilPixelFormat: MTLPixelFormat

The format used to generate the depthStencilTexture object.

var depthStencilAttachmentTextureUsage: MTLTextureUsage

The texture usage characteristics that the view uses when creating the depth and stencil textures.

var clearDepth: Double

The depth value to use to clear the depth target when creating a render pass descriptor.

