

- Metal
- MTLRenderPassAttachmentDescriptor
-  level 

Instance Property

# level

The mipmap level of the texture used for rendering to the attachment.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var level: Int { get set }
```

## Discussion

The default value is `0`.

## See Also

### Specifying the Texture for the Attachment

var texture: (any MTLTexture)?

The texture object associated with this attachment.

var slice: Int

The slice of the texture used for rendering to the attachment.

var depthPlane: Int

The depth plane of the texture used for rendering to the attachment.

