

- Metal
- MTLRenderPassColorAttachmentDescriptorArray
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns the descriptor object for the specified color attachment.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
subscript(attachmentIndex: Int) -> MTLRenderPassColorAttachmentDescriptor! { get set }
```

## Parameters 

`attachmentIndex`  

An index in the color attachment array.

## Return Value

A descriptor object that contains color attachment information.

