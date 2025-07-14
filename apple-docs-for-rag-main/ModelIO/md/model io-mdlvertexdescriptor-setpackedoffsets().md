

- Model I/O
- MDLVertexDescriptor
-  setPackedOffsets() 

Instance Method

# setPackedOffsets()

Sets the offset for each vertex attribute to the minimum value to pack vertex data together in a single buffer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func setPackedOffsets()
```

## Discussion

This method examines the stride property of each of the descriptor’s vertex buffer layouts, calculates an offset for each of the descriptor’s vertex attributes that fits vertex data into a single buffer with minimal unused padding space between attributes, then sets the offset property of each vertex attribute to the calculated value.

For example, consider a vertex buffer with three attributes: position, normal, and texture coordinates. The position and normal attributes each contain 3-component floating-point vectors for each vertex, and the texture coordinate attribute contains a 2-component floating-point vector for each vertex. The default stride for the each of the first two attributes is 12 bytes (4 bytes per component), and the default stride for the third is 8 bytes (4 bytes per component). Therefore, to pack data for the attributes together in the same vertex buffer, the offest for the position attribute is 0, the offset for the normal attribute is 12 (the width of the first attribute), and the offset of the texture coordinate attribute is 24 (the combined width of the first two attributes).

To describe a fully packed vertex buffer, call this method *before* calling the setPackedStrides() method.

## See Also

### Working with Vertex Attributes

var attributes: NSMutableArray

The list of vertex attributes described by the vertex descriptor.

func attributeNamed(String) -> MDLVertexAttribute?

Returns the vertex attribute with the specified name in the vertex descriptor.

func addOrReplaceAttribute(MDLVertexAttribute)

Adds the specified vertex attribute to the vertex descriptor, replacing any existing attribute with the same name.

