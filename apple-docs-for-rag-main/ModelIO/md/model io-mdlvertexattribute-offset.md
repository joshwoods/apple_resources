

- Model I/O
- MDLVertexAttribute
-  offset 

Instance Property

# offset

The offset, in bytes, of vertex data for the attribute in a vertex buffer, relative to the start of data for each vertex.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var offset: Int { get set }
```

## Discussion

For example, if a vertex buffer contains interleaved data for two attributes, the first attribute’s offset is typically zero, and the second attribute’s offset is at least the data size of the first attribute.

## See Also

### Inspecting a Vertex Attribute

var name: String

An identifier for the semantic use of the vertex attribute.

var format: MDLVertexFormat

The format of per-vertex data for the attribute.

var bufferIndex: Int

The index of the vertex buffer containing data for this attribute in a mesh’s vertexBuffers array.

var initializationValue: vector_float4

The default value for vertex data for this attribute.

