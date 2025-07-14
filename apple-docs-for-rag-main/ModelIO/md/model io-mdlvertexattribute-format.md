

- Model I/O
- MDLVertexAttribute
-  format 

Instance Property

# format

The format of per-vertex data for the attribute.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var format: MDLVertexFormat { get set }
```

## Discussion

A MDLVertexFormat value describes the number of vector components for an attribute, as well as the data type of each component, and, for special packed formats, the layout of components.

## See Also

### Inspecting a Vertex Attribute

var name: String

An identifier for the semantic use of the vertex attribute.

var offset: Int

The offset, in bytes, of vertex data for the attribute in a vertex buffer, relative to the start of data for each vertex.

var bufferIndex: Int

The index of the vertex buffer containing data for this attribute in a mesh’s vertexBuffers array.

var initializationValue: vector_float4

The default value for vertex data for this attribute.

