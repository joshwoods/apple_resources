

- Metal
- MTLRenderCommandEncoder
-  drawPrimitives(type:indirectBuffer:indirectBufferOffset:) 

Instance Method

# drawPrimitives(type:indirectBuffer:indirectBufferOffset:)

Encodes a draw command that renders multiple instances of a geometric primitive with indirect arguments.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func drawPrimitives(
    type primitiveType: MTLPrimitiveType,
    indirectBuffer: any MTLBuffer,
    indirectBufferOffset: Int
)
```

**Required**

## Parameters 

`primitiveType`  

An MTLPrimitiveType instance that represents how the command interprets vertex argument data.

See the setVertexBuffer(_:offset:index:) method and its siblings for more information about setting an entry in the vertex shader argument table for buffers.

`indirectBuffer`  

An MTLBuffer instance with data that matches the layout of the MTLDrawPrimitivesIndirectArguments structure.

`indirectBufferOffset`  

An integer that represents the location, in bytes, from the start of `indirectBuffer` where the indirect arguments structure begins.

See the Metal feature set tables (PDF) to check for offset alignment requirements for buffers in `device` and `constant` address space.

## Discussion

Indirect drawing methods may help your app avoid expensive latency costs. This is because the command reads arguments from an MTLBuffer instance instead of using the CPU to pass parameters to the command.

The method records the encoder’s current rendering state and resources the command needs as it runs. You can safely change the encoder’s render pipeline state to encode other commands after calling this method. Subsequent changes to the state don’t affect the commands already in the encoder’s MTLCommandBuffer.

## See Also

### Drawing with Vertices

func drawPrimitives(type: MTLPrimitiveType, vertexStart: Int, vertexCount: Int)

Encodes a draw command that renders an instance of a geometric primitive.

**Required**

func drawPrimitives(type: MTLPrimitiveType, vertexStart: Int, vertexCount: Int, instanceCount: Int)

Encodes a draw command that renders multiple instances of a geometric primitive.

**Required**

func drawPrimitives(type: MTLPrimitiveType, vertexStart: Int, vertexCount: Int, instanceCount: Int, baseInstance: Int)

Encodes a draw command that renders multiple instances of a geometric primitive that starts with a custom instance identification number.

**Required**

