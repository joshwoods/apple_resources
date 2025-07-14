

- Metal
- MTLDevice
-  makeIndirectCommandBuffer(descriptor:maxCommandCount:options:) 

Instance Method

# makeIndirectCommandBuffer(descriptor:maxCommandCount:options:)

Creates an indirect command buffer instance.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
func makeIndirectCommandBuffer(
    descriptor: MTLIndirectCommandBufferDescriptor,
    maxCommandCount maxCount: Int,
    options: MTLResourceOptions = []
) -> (any MTLIndirectCommandBuffer)?
```

**Required**

## Parameters 

`descriptor`  

An MTLIndirectCommandBufferDescriptor instance.

`maxCount`  

The largest number of commands you can store in the buffer.

`options`  

An MTLResourceOptions instance.

## Return Value

A new MTLIndirectCommandBuffer instance if the method completed successfully; otherwise `nil`.

## Mentioned in 

Creating an Indirect Command Buffer

