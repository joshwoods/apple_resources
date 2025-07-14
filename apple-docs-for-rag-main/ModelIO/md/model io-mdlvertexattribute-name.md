

- Model I/O
- MDLVertexAttribute
-  name 

Instance Property

# name

An identifier for the semantic use of the vertex attribute.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var name: String { get set }
```

## Discussion

Depending on the source of data for a mesh—that is, which file format it was loaded from in a MDLAsset object, or whether it was programmatically created—a vertex attribute’s name can be either one of the constants listed in Vertex Attributes or an identifier specific to the file format.

## See Also

### Inspecting a Vertex Attribute

var format: MDLVertexFormat

The format of per-vertex data for the attribute.

var offset: Int

The offset, in bytes, of vertex data for the attribute in a vertex buffer, relative to the start of data for each vertex.

var bufferIndex: Int

The index of the vertex buffer containing data for this attribute in a mesh’s vertexBuffers array.

var initializationValue: vector_float4

The default value for vertex data for this attribute.

