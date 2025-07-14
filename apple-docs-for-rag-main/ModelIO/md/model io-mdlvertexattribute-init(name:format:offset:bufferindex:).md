

- Model I/O
- MDLVertexAttribute
-  init(name:format:offset:bufferIndex:) 

Initializer

# init(name:format:offset:bufferIndex:)

Initializes a vertex attribute object with the specified property values.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    name: String,
    format: MDLVertexFormat,
    offset: Int,
    bufferIndex: Int
)
```

## Parameters 

`name`  

An identifier for the semantic use of the vertex attribute.

`format`  

The format of per-vertex data for the attribute.

`offset`  

The offset, in bytes, of vertex data for the attribute in a vertex buffer, relative to the start of data for each vertex.

`bufferIndex`  

The index of the vertex buffer containing data for this attribute in a mesh’s vertexBuffers array.

## Return Value

A new vertex attribute object.

## Discussion

Use this initializer when constructing a new mesh from custom data, or when building a new MDLVertexDescriptor object to change the vertex buffer formatting of an existing mesh. When you load a mesh from a MDLAsset object, Model I/O automatically creates vertex descriptor and vertex attribute objects describing the mesh’s vertex data.

