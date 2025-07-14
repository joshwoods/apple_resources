

- Metal
- MTLVertexAttributeDescriptor
-  bufferIndex 

Instance Property

# bufferIndex

The index in the argument table for the associated vertex buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var bufferIndex: Int { get set }
```

## See Also

### Related Documentation

func setVertexBuffer((any MTLBuffer)?, offset: Int, index: Int)

Assigns a buffer to an entry in the vertex shader argument table.

**Required**

### Organizing the Vertex Attribute

var format: MTLVertexFormat

The format of the vertex attribute.

var offset: Int

The location of an attribute in vertex data, determined by the byte offset from the start of the vertex data.

