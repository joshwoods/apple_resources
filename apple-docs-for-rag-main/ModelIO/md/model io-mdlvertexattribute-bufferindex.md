

- Model I/O
- MDLVertexAttribute
-  bufferIndex 

Instance Property

# bufferIndex

The index of the vertex buffer containing data for this attribute in a mesh’s vertexBuffers array.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var bufferIndex: Int { get set }
```

## Discussion

A mesh may store vertex data in either a *structure of arrays* model, where data for each attribute lies in a separate vertex buffer, or in an *array of structures* model. In the latter, multiple vertex attributes share the same buffer (and thus have the same bufferIndex value), and the format and offset values (together with the stride value of a related MDLVertexBufferLayout object) identify which bytes in that buffer refer to which vertex attributes.

## See Also

### Inspecting a Vertex Attribute

var name: String

An identifier for the semantic use of the vertex attribute.

var format: MDLVertexFormat

The format of per-vertex data for the attribute.

var offset: Int

The offset, in bytes, of vertex data for the attribute in a vertex buffer, relative to the start of data for each vertex.

var initializationValue: vector_float4

The default value for vertex data for this attribute.

