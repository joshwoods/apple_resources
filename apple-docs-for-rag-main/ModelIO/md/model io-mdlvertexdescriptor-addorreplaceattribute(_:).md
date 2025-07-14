

- Model I/O
- MDLVertexDescriptor
-  addOrReplaceAttribute(\_:) 

Instance Method

# addOrReplaceAttribute(\_:)

Adds the specified vertex attribute to the vertex descriptor, replacing any existing attribute with the same name.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func addOrReplaceAttribute(_ attribute: MDLVertexAttribute)
```

## Parameters 

`attribute`  

The vertex attribute to add to the vertex descriptor.

## Discussion

If the vertex descriptor contains an attribute whose name property is the same as that of the `attribute` parameter, the new attribute replaces the existing attribute in the attributes array. Otherwise, this method adds the new attribute to the end of the attributes array.

## See Also

### Working with Vertex Attributes

var attributes: NSMutableArray

The list of vertex attributes described by the vertex descriptor.

func attributeNamed(String) -> MDLVertexAttribute?

Returns the vertex attribute with the specified name in the vertex descriptor.

func setPackedOffsets()

Sets the offset for each vertex attribute to the minimum value to pack vertex data together in a single buffer.

