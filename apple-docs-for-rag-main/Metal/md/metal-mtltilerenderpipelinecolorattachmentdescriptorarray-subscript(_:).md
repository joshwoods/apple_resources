

- Metal
- MTLTileRenderPipelineColorAttachmentDescriptorArray
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns the render pipeline state for the specified color attachment.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS 1.0+

``` source
subscript(attachmentIndex: Int) -> MTLTileRenderPipelineColorAttachmentDescriptor { get set }
```

## Parameters 

`attachmentIndex`  

An index in the color attachment array.

## Return Value

A MTLTileRenderPipelineColorAttachmentDescriptor that describes the render pipeline information for a color attachment.

