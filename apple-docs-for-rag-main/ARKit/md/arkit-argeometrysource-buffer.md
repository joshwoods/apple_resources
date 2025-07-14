

- ARKit
- ARGeometrySource
-  buffer 

Instance Property

# buffer

A Metal buffer that contains a list of vectors.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
var buffer: any MTLBuffer { get }
```

## Discussion

Each vector in the buffer is of the type defined by format. Every vector may itself contain multiple scalars, defined by componentsPerVector.

The buffer’s storageMode is MTLStorageMode.shared which allows it to be accessed on both, the CPU, and GPU.

## See Also

### Accessing Geometry

subscript(Int32) -> (Float, Float, Float)

Provides the source float triplet at the subscripted index.

subscript(Int32) -> CUnsignedChar

Provides the number at the subscripted index.

