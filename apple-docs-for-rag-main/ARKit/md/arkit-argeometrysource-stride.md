

- ARKit
- ARGeometrySource
-  stride 

Instance Property

# stride

The length, in bytes, of the start of one vector in the buffer to the start of the next vector.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
var stride: Int { get }
```

## Discussion

Stride may contain padding, so it’s not always equal to the vector-format’s total size in bytes.

## See Also

### Getting Geometry Information

var componentsPerVector: Int

The number of scalar components in each vector.

var count: Int

The number of vectors in the buffer.

var format: MTLVertexFormat

The type of vector data in the buffer.

var offset: Int

The offset, in bytes, from the beginning of the buffer.

