

- Metal
- MTLRenderPassStencilAttachmentDescriptor
-  clearStencil 

Instance Property

# clearStencil

The value to use when clearing the stencil attachment.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var clearStencil: UInt32 { get set }
```

## Discussion

If the loadAction property of the attachment is set to MTLLoadAction.clear, then at the start of a render pass, the GPU fills the contents of the attachment with the value stored in the clearStencil property. Otherwise, the GPU ignores clearStencil.

The default value is `0`.

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

