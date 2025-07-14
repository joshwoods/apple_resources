

- Metal
- MTLRenderCommandEncoder
-  drawIndexedPrimitives(type:indexCount:indexType:indexBuffer:indexBufferOffset:instanceCount:baseVertex:baseInstance:) 

Instance Method

# drawIndexedPrimitives(type:indexCount:indexType:indexBuffer:indexBufferOffset:instanceCount:baseVertex:baseInstance:)

Encodes a draw command that renders multiple instances of a geometric primitive with indexed vertices, starting with a custom vertex and instance.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func drawIndexedPrimitives(
    type primitiveType: MTLPrimitiveType,
    indexCount: Int,
    indexType: MTLIndexType,
    indexBuffer: any MTLBuffer,
    indexBufferOffset: Int,
    instanceCount: Int,
    baseVertex: Int,
    baseInstance: Int
)
```

**Required**

## Parameters 

`primitiveType`  

An MTLPrimitiveType instance that represents how the command interprets vertex argument data.

See the setVertexBuffer(_:offset:index:) method and its siblings for more information about setting an entry in the vertex shader argument table for buffers.

`indexCount`  

An integer that represents the number of vertices the command reads from `indexBuffer` for each instance.

`indexType`  

An MTLIndexType instance that represents the index’s format, including MTLIndexType.uint16 and MTLIndexType.uint32.

`indexBuffer`  

An MTLBuffer instance that contains the `indexCount` vertex indices of the `indexType` format.

`indexBufferOffset`  

An integer that represents the location that’s a multiple of 4 bytes from the start of `indexBuffer` where the vertex indices begin.

`instanceCount`  

An integer that represents the number of times the command draws `primitiveType` with `indexCount` vertices.

`baseVertex`  

The lowest value the command passes to your vertex shader’s parameter with the `vertex_id` attribute. The command assigns each vertex a unique `vertex_id` value that increases from `baseVertex` through `(baseVertex + indexCount - 1)`. Your shader can use that value to identify each vertex in the `primitiveType` instance.

For more information about the `vertex_id` argument attribute for vertex shaders, see the Metal Shading Language Specification (PDF).

`baseInstance`  

The lowest value the command passes to your vertex shader’s parameter with the `instance_id` attribute.

The command assigns each drawing instance a unique `instance_id` value that increases from `baseInstance` through `(baseInstance + instanceCount - 1)`. Your shader can use that value to identify which instance the vertex belongs to.

For more information about the `instance_id` argument attribute for vertex shaders, see the Metal Shading Language Specification (PDF).

## Discussion

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

func drawIndexedPrimitives(type: MTLPrimitiveType, indexType: MTLIndexType, indexBuffer: any MTLBuffer, indexBufferOffset: Int, indirectBuffer: any MTLBuffer, indirectBufferOffset: Int)

Encodes a draw command that renders multiple instances of a geometric primitive with indexed vertices and indirect arguments.

**Required**

