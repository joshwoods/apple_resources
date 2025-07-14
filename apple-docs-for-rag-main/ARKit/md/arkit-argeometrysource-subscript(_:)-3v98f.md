

- ARKit
- ARGeometrySource
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Provides the source float triplet at the subscripted index.

iOS 14.0+iPadOS 14.0+

``` source
@nonobjc
subscript(index: Int32) -> (Float, Float, Float) { get }
```

## Discussion

This subscript operates on three-component geometry sources with a format of MTLVertexFormat.float3. This operator returns an (x, y, z) offset relative to its parent anchor’s position that corresponds to the subscripted vertex position in vertices and to the subscripted normal vector in normals.

## See Also

### Accessing Geometry

subscript(Int32) -> CUnsignedChar

Provides the number at the subscripted index.

var buffer: any MTLBuffer

A Metal buffer that contains a list of vectors.

