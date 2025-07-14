

- Metal
- MTLRenderPipelineColorAttachmentDescriptorArray
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns the render pipeline state for the specified color attachment.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
subscript(attachmentIndex: Int) -> MTLRenderPipelineColorAttachmentDescriptor! { get set }
```

## Parameters 

`attachmentIndex`  

An index in the color attachment array.

## Return Value

A MTLRenderPipelineColorAttachmentDescriptor object that describes the render pipeline information for a color attachment.

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

