

- MetalKit
- MTKView
-  depthStencilPixelFormat 

Instance Property

# depthStencilPixelFormat

The format used to generate the depthStencilTexture object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var depthStencilPixelFormat: MTLPixelFormat { get set }
```

## Discussion

The default value is MTLPixelFormat.invalid, which means that the view doesn’t create a depth and stencil texture. If you set it to a different format, the view automatically creates those textures for you and configures them as part of any render passes that the view creates.

## See Also

### Configuring the Render Target Properties

var depthStencilAttachmentTextureUsage: MTLTextureUsage

The texture usage characteristics that the view uses when creating the depth and stencil textures.

var clearDepth: Double

The depth value to use to clear the depth target when creating a render pass descriptor.

var clearStencil: UInt32

The stencil value to use to clear the stencil target when creating a render pass descriptor.

