

- Metal
- MTLRenderPassAttachmentDescriptor
-  depthPlane 

Instance Property

# depthPlane

The depth plane of the texture used for rendering to the attachment.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var depthPlane: Int { get set }
```

## Discussion

If the texture isn’t a 3D texture, then Metal ignores this property.

The default value is `0`.

## See Also

### Specifying the Texture for the Attachment

var texture: (any MTLTexture)?

The texture object associated with this attachment.

var level: Int

The mipmap level of the texture used for rendering to the attachment.

var slice: Int

The slice of the texture used for rendering to the attachment.

