

- Metal
- MTLRenderPipelineDescriptor
-  stencilAttachmentPixelFormat 

Instance Property

# stencilAttachmentPixelFormat

The pixel format of the attachment that stores stencil data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var stencilAttachmentPixelFormat: MTLPixelFormat { get set }
```

## Discussion

By default, the pixel format of the rendering pipeline state for each attachment is `MTLPixelFormatInvalid`.

## See Also

### Specifying Rendering Pipeline State

func reset()

Specifies the default rendering pipeline state values for the descriptor.

var colorAttachments: MTLRenderPipelineColorAttachmentDescriptorArray

An array of attachments that store color data.

var depthAttachmentPixelFormat: MTLPixelFormat

The pixel format of the attachment that stores depth data.

