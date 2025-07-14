

- Model I/O
- MDLVertexDescriptor
-  attributeNamed(\_:) 

Instance Method

# attributeNamed(\_:)

Returns the vertex attribute with the specified name in the vertex descriptor.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func attributeNamed(_ name: String) -> MDLVertexAttribute?
```

## Parameters 

`name`  

The attribute name for which to retrieve data. See Vertex Attributes for standard attribute names.

## Return Value

The descriptor’s vertex attribute with the specified name, or `nil` if the attributes array does not contain a vertex attribute with that name.

## See Also

### Working with Vertex Attributes

var attributes: NSMutableArray

The list of vertex attributes described by the vertex descriptor.

func addOrReplaceAttribute(MDLVertexAttribute)

Adds the specified vertex attribute to the vertex descriptor, replacing any existing attribute with the same name.

func setPackedOffsets()

Sets the offset for each vertex attribute to the minimum value to pack vertex data together in a single buffer.

