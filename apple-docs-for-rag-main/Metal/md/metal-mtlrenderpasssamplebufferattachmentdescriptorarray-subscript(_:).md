

- Metal
- MTLRenderPassSampleBufferAttachmentDescriptorArray
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns the descriptor object for the specified sample buffer attachment.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
subscript(attachmentIndex: Int) -> MTLRenderPassSampleBufferAttachmentDescriptor! { get set }
```

## Parameters 

`attachmentIndex`  

An index for the object to fetch.

## Return Value

The MTLRenderPassSampleBufferAttachmentDescriptor at the specified index.

