

- Model I/O
- MDLVertexDescriptor
-  attributes 

Instance Property

# attributes

The list of vertex attributes described by the vertex descriptor.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var attributes: NSMutableArray { get set }
```

## Discussion

A MDLVertexAttribute object describes the data for one semantic attribute of a vertex, such as position, normal, color, or texture coordinates. Each object names the semantic attribute it is used for, and describes the format of the data for that attribute and its location in the vertex buffers of a MDLMesh object.

The order of objects in this array reflects the order of vertex attribute data in the vertex buffer(s) of the mesh described by this vertex descriptor. For example, if this array contains a vertex attribute whose name is MDLVertexAttributePosition, followed by an attribute named MDLVertexAttributeNormal, followed by an attribute named MDLVertexAttributeTextureCoordinate, and the mesh contains a single vertex buffer, each entry in that vertex buffer consists of position data, then normal data, then texture coordinate data.

## See Also

### Working with Vertex Attributes

func attributeNamed(String) -> MDLVertexAttribute?

Returns the vertex attribute with the specified name in the vertex descriptor.

func addOrReplaceAttribute(MDLVertexAttribute)

Adds the specified vertex attribute to the vertex descriptor, replacing any existing attribute with the same name.

func setPackedOffsets()

Sets the offset for each vertex attribute to the minimum value to pack vertex data together in a single buffer.

