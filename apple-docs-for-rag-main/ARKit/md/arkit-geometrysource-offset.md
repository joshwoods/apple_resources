

- ARKit
- GeometrySource
-  offset 

Instance Property

# offset

The offset, in bytes, from the beginning of a geometry source’s buffer.

visionOS 1.0+

``` source
var offset: Int { get }
```

## See Also

### Inspecting geometry data

var buffer: any MTLBuffer

A Metal buffer that contains per-vector data for a geometry source.

var count: Int

The number of vectors in a geometry source.

var format: MTLVertexFormat

The vertex format for data in a geometry source’s buffer.

var componentsPerVector: Int

The number of scalar components in each vector in a geometry source.

var stride: Int

The number of bytes between one vector and another in a geometry source’s buffer.

var description: String

A textual representation of this geometry source.

