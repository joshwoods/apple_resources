

- Metal
- MTLArgumentEncoder
-  setIndirectCommandBuffers(\_:range:) 

Instance Method

# setIndirectCommandBuffers(\_:range:)

Encodes an array of indirect command buffers into the argument buffer.

iOS 12.0+iPadOS 12.0+Mac CatalystmacOS 10.14+tvOS 12.0+visionOS

``` source
func setIndirectCommandBuffers(
    _ buffers: [(any MTLIndirectCommandBuffer)?],
    range: Range
)
```

## Parameters 

`buffers`  

An array of indirect command buffers the method encodes.

`range`  

A range of indices within the argument buffer for each element in `buffers`. The values correspond to either the index IDs of declarations in Metal Shading Language (MSL) or the index property of MTLArgumentDescriptor instances.

## See Also

### Encoding Indirect Command Buffers

func setIndirectCommandBuffer((any MTLIndirectCommandBuffer)?, index: Int)

Encodes a reference to an indirect command buffer into the argument buffer.

**Required**

