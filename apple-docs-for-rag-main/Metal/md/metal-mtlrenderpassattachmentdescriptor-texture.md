

- Metal
- MTLRenderPassAttachmentDescriptor
-  texture 

Instance Property

# texture

The texture object associated with this attachment.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var texture: (any MTLTexture)? { get set }
```

## Mentioned in 

Setting Load and Store Actions

Choosing a Resource Storage Mode for Apple GPUs

## Discussion

You must set the attachment’s `texture` property, choosing an appropriate pixel format for the texture.

- To store color values in an attachment, use a texture with a color-renderable pixel format.

- To store depth values, use a texture with a depth-renderable pixel format, such as MTLPixelFormat.depth32Float.

- To store stencil values, use a texture with a stencil-renderable pixel format, such as MTLPixelFormat.stencil8.

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

### Specifying the Texture for the Attachment

var level: Int

The mipmap level of the texture used for rendering to the attachment.

var slice: Int

The slice of the texture used for rendering to the attachment.

var depthPlane: Int

The depth plane of the texture used for rendering to the attachment.

