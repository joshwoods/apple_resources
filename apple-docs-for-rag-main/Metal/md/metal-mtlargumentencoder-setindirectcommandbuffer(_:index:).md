

- Metal
- MTLArgumentEncoder
-  setIndirectCommandBuffer(\_:index:) 

Instance Method

# setIndirectCommandBuffer(\_:index:)

Encodes a reference to an indirect command buffer into the argument buffer.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
func setIndirectCommandBuffer(
    _ indirectCommandBuffer: (any MTLIndirectCommandBuffer)?,
    index: Int
)
```

**Required**

## Parameters 

`indirectCommandBuffer`  

An indirect command-buffer the method encodes.

`index`  

The index of an inline, constant-data argument within the argument buffer. The value corresponds to either the index ID of a declaration in Metal Shading Language (MSL) or the index property of an MTLArgumentDescriptor instance.

## See Also

### Encoding Indirect Command Buffers

func setIndirectCommandBuffers([(any MTLIndirectCommandBuffer)?], range: Range&lt;Int>)

Encodes an array of indirect command buffers into the argument buffer.

