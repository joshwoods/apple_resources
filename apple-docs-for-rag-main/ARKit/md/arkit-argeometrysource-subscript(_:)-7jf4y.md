

- ARKit
- ARGeometrySource
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Provides the number at the subscripted index.

iOS 14.0+iPadOS 14.0+

``` source
@nonobjc
subscript(index: Int32) -> CUnsignedChar { get }
```

## Discussion

This subscript operates on one-component geometry sources with a format of MTLVertexFormat.uchar, such as classification.

## See Also

### Accessing Geometry

subscript(Int32) -> (Float, Float, Float)

Provides the source float triplet at the subscripted index.

var buffer: any MTLBuffer

A Metal buffer that contains a list of vectors.

