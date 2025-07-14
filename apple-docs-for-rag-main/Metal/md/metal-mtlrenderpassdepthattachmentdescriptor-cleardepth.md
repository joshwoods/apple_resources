

- Metal
- MTLRenderPassDepthAttachmentDescriptor
-  clearDepth 

Instance Property

# clearDepth

The depth to use when clearing the depth attachment.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var clearDepth: Double { get set }
```

## Discussion

If the loadAction property of the attachment is set to MTLLoadAction.clear, then at the start of a render pass, the GPU fills the contents of the attachment with the value stored in the clearDepth property. Otherwise, the GPU ignores clearDepth.

The default value is `1.0`.

