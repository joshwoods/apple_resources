

- Metal
- MTLVertexAttributeDescriptor
-  offset 

Instance Property

# offset

The location of an attribute in vertex data, determined by the byte offset from the start of the vertex data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var offset: Int { get set }
```

## Discussion

The `offset` value must be a multiple of `4` bytes.

## See Also

### Organizing the Vertex Attribute

var format: MTLVertexFormat

The format of the vertex attribute.

var bufferIndex: Int

The index in the argument table for the associated vertex buffer.

