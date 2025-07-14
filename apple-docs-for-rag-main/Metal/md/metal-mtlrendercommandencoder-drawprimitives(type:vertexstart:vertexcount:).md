

- Metal
- MTLRenderCommandEncoder
-  drawPrimitives(type:vertexStart:vertexCount:) 

Instance Method

# drawPrimitives(type:vertexStart:vertexCount:)

Encodes a draw command that renders an instance of a geometric primitive.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func drawPrimitives(
    type primitiveType: MTLPrimitiveType,
    vertexStart: Int,
    vertexCount: Int
)
```

**Required**

## Parameters 

`primitiveType`  

An MTLPrimitiveType instance that represents how the command interprets vertex argument data.

See the setVertexBuffer(_:offset:index:) method and its siblings for more information about setting an entry in the vertex shader argument table for buffers.

`vertexStart`  

The lowest value the command passes to your vertex shader’s parameter with the `vertex_id` attribute. The command assigns each vertex a unique `vertex_id` value within its drawing instance that increases from `vertexStart` through `(vertexStart + vertexCount - 1)`. Your shader can use that value to identify a vertex in each drawing instance.

For more information about the `vertex_id` argument attribute for vertex shaders, see the Metal Shading Language Specification (PDF).

`vertexCount`  

An integer that represents the number of vertices of `primitiveType` the command draws.

## Discussion

The method records the encoder’s current rendering state and resources the command needs as it runs. You can safely change the encoder’s render pipeline state to encode other commands after calling this method. Subsequent changes to the state don’t affect the commands already in the encoder’s MTLCommandBuffer.

## See Also

### Drawing with Vertices

func drawPrimitives(type: MTLPrimitiveType, vertexStart: Int, vertexCount: Int, instanceCount: Int)

Encodes a draw command that renders multiple instances of a geometric primitive.

**Required**

func drawPrimitives(type: MTLPrimitiveType, vertexStart: Int, vertexCount: Int, instanceCount: Int, baseInstance: Int)

Encodes a draw command that renders multiple instances of a geometric primitive that starts with a custom instance identification number.

**Required**

func drawPrimitives(type: MTLPrimitiveType, indirectBuffer: any MTLBuffer, indirectBufferOffset: Int)

Encodes a draw command that renders multiple instances of a geometric primitive with indirect arguments.

**Required**

