

- Model I/O
- MDLSubmeshTopology
-  faceTopology 

Instance Property

# faceTopology

A buffer identifying the faces in the submesh and the number of vertices in each.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var faceTopology: (any MDLMeshBuffer)? { get set }
```

## Discussion

This buffer contains 8-bit unsigned integer values, where each entry corresponds to the number of vertices making up a face. For example, a submesh containing two triangles, a quad, and a line would contain the data `3 3 4 2`. If the submesh’s geometryType property identifies a fixed type (such as MDLGeometryType.triangles), this buffer is optional. In this case, Model I/O automatically creates the buffer upon the first attempt to read this property.

The submesh’s indexBuffer property stores indices in the order described by the topology buffer. In the example above, the index buffer would contain three indices for the first triangle, followed by three for the second, followed by four for the quad, and finally two indices for the line.

## See Also

### Identifying Faces

var faceCount: Int

The number of faces in the submesh’s face topology buffer.

