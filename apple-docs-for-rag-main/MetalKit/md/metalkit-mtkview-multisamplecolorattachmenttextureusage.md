

- MetalKit
- MTKView
-  multisampleColorAttachmentTextureUsage 

Instance Property

# multisampleColorAttachmentTextureUsage

The texture usage characteristics that the view uses when creating multisample textures.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var multisampleColorAttachmentTextureUsage: MTLTextureUsage { get set }
```

## Discussion

The default value is renderTarget.

## See Also

### Configuring Multisampling

var sampleCount: Int

The sample count used to generate the multisampleColorTexture object.

