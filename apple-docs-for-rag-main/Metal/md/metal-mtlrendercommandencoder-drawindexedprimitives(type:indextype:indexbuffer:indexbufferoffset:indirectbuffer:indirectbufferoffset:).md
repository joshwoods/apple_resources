

- Metal
- MTLRenderCommandEncoder
-  drawIndexedPrimitives(type:indexType:indexBuffer:indexBufferOffset:indirectBuffer:indirectBufferOffset:) 

Instance Method

# drawIndexedPrimitives(type:indexType:indexBuffer:indexBufferOffset:indirectBuffer:indirectBufferOffset:)

Encodes a draw command that renders multiple instances of a geometric primitive with indexed vertices and indirect arguments.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func drawIndexedPrimitives(
    type primitiveType: MTLPrimitiveType,
    indexType: MTLIndexType,
    indexBuffer: any MTLBuffer,
    indexBufferOffset: Int,
    indirectBuffer: any MTLBuffer,
    indirectBufferOffset: Int
)
```

**Required**

## Parameters 

`primitiveType`  

An MTLPrimitiveType instance that represents how the command interprets vertex argument data.

See the setVertexBuffer(_:offset:index:) method and its siblings for more information about setting an entry in the vertex shader argument table for buffers.

`indexType`  

An MTLIndexType instance that represents the index’s format, including MTLIndexType.uint16 and MTLIndexType.uint32.

`indexBuffer`  

An MTLBuffer instance that contains thevertex indices of the `indexType` format.

`indexBufferOffset`  

An integer that represents the location that’s a multiple of 4 bytes from the start of `indexBuffer` where the vertex indices begin.

`indirectBuffer`  

An MTLBuffer instance with data that matches the layout of the MTLDrawIndexedPrimitivesIndirectArguments structure.

`indirectBufferOffset`  

An integer that represents the location, in bytes, from the start of `indirectBuffer` where the indirect arguments structure begins.

See the Metal feature set tables (PDF) to check for offset alignment requirements for buffers in `device` and `constant` address space.

## Discussion

Indirect drawing methods may help your app avoid expensive latency costs. This is because the command reads arguments from an MTLBuffer instance instead of using the CPU to pass parameters to the command.

You can complete a primitive and start a new one by passing a sentinel index value that’s the largest unsigned integer possible for `indexType`. For example, the largest unsigned integer for MTLIndexType.uint16 and MTLIndexType.uint32 is `0xFFFF` and `0xFFFFFFFF`, respectively. The command finishes the current primitive and begins drawing a new one each time the command reads a sentinel index value.

The method records the encoder’s current rendering state and resources the command needs as it runs. You can safely change the encoder’s render pipeline state to encode other commands after calling this method. Subsequent changes to the state don’t affect the commands already in the encoder’s MTLCommandBuffer.

## See Also

### Drawing with Indexed Vertices

func drawIndexedPrimitives(type: MTLPrimitiveType, indexCount: Int, indexType: MTLIndexType, indexBuffer: any MTLBuffer, indexBufferOffset: Int)

Encodes a draw command that renders an instance of a geometric primitive with indexed vertices.

**Required**

func drawIndexedPrimitives(type: MTLPrimitiveType, indexCount: Int, indexType: MTLIndexType, indexBuffer: any MTLBuffer, indexBufferOffset: Int, instanceCount: Int)

Encodes a draw command that renders multiple instances of a geometric primitive with indexed vertices.

**Required**

func drawIndexedPrimitives(type: MTLPrimitiveType, indexCount: Int, indexType: MTLIndexType, indexBuffer: any MTLBuffer, indexBufferOffset: Int, instanceCount: Int, baseVertex: Int, baseInstance: Int)

Encodes a draw command that renders multiple instances of a geometric primitive with indexed vertices, starting with a custom vertex and instance.

**Required**

