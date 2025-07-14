

- ARKit
- ARGeometrySource
-  componentsPerVector 

Instance Property

# componentsPerVector

The number of scalar components in each vector.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
var componentsPerVector: Int { get }
```

## Discussion

In the case that componentsPerVector is greater than 1, the element type of the geometry-source array is itself, a sequence.

## See Also

### Getting Geometry Information

var count: Int

The number of vectors in the buffer.

var format: MTLVertexFormat

The type of vector data in the buffer.

var offset: Int

The offset, in bytes, from the beginning of the buffer.

var stride: Int

The length, in bytes, of the start of one vector in the buffer to the start of the next vector.

