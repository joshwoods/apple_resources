

- MetalKit
- MTKView
-  sampleCount 

Instance Property

# sampleCount

The sample count used to generate the multisampleColorTexture object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var sampleCount: Int { get set }
```

## Discussion

Support for different sample count values varies by device object. Call the supportsTextureSampleCount(_:) method to determine if the device object supports the sample count you want.

The default value is `1`. When you set a value greater than `1`, the view creates and configures an intermediate set of multisample textures. The pixel format is the same as the one specified for the drawable; see colorPixelFormat. When the view creates a render pass descriptor, the render pass uses those intermediate textures as the color render targets, with a store action to resolve these multisample textures into the drawable’s texture (MTLStoreAction.multisampleResolve).

## See Also

### Configuring Multisampling

var multisampleColorAttachmentTextureUsage: MTLTextureUsage

The texture usage characteristics that the view uses when creating multisample textures.

