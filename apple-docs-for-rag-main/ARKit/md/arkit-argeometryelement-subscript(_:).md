

- ARKit
- ARGeometryElement
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Provides an array of vertex indices that respresents the geometric primitive at the subscripted index.

iOS 14.0+iPadOS 14.0+

``` source
@nonobjc
subscript(index: Int) -> [Int32] { get }
```

## Discussion

This subscript operates on geometry elements of type Int32 with `4` bytesPerIndex. In the case of the faces property, this operator returns an array of size `3`. The contents of the array are vertex indices that compose a triangle primitive, which represents the face identified by the argument face index.

## See Also

### Accessing Index Data

var buffer: any MTLBuffer

A Metal buffer containing primitive data.

