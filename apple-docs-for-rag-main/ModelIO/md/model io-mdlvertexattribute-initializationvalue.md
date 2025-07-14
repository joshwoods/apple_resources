

- Model I/O
- MDLVertexAttribute
-  initializationValue 

Instance Property

# initializationValue

The default value for vertex data for this attribute.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var initializationValue: vector_float4 { get set }
```

## Discussion

When you set the vertexDescriptor property of a MDLMesh object, the mesh automatically formats its vertex buffers to match the new descriptor. If the vertex descriptor contains a vertex attribute that is not already present in the mesh, the mesh creates a new vertex buffer (or allocates space in an interleaved vertex buffer, if the vertex descriptor describes such) for the new attribute, and fills in per-vertex data for that attribute using this property’s value.

Although this property’s type is `vector_float4`, Model I/O uses only the components of the vector that match the vertex attribute’s format property. For example, if you set this property’s value to the vector `{1, 2, 3, 4}` on a vertex attribute whose format is MDLVertexFormat.float2, each vertex will be initialized with the value `{1, 2}`.

The default initialization value is the vector `{0, 0, 0, 1}`.

## See Also

### Inspecting a Vertex Attribute

var name: String

An identifier for the semantic use of the vertex attribute.

var format: MDLVertexFormat

The format of per-vertex data for the attribute.

var offset: Int

The offset, in bytes, of vertex data for the attribute in a vertex buffer, relative to the start of data for each vertex.

var bufferIndex: Int

The index of the vertex buffer containing data for this attribute in a mesh’s vertexBuffers array.

