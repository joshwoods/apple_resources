

- SceneKit
- SCNGeometrySource
-  dataStride 

Instance Property

# dataStride

The number of bytes from a vector to the next one in the data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var dataStride: Int { get }
```

## Discussion

You can use the SCNGeometrySource and SCNGeometrySource parameters can together to interleave data for multiple geometry sources in the same array, improving rendering performance. See SCNGeometrySource for details.

## See Also

### Inspecting a Geometry Source

var data: Data

The data for the geometry source.

var semantic: SCNGeometrySource.Semantic

The semantic value (or attribute) the geometry source describes for each vertex.

var vectorCount: Int

The number of vectors in the data.

var usesFloatComponents: Bool

A Boolean value that indicates whether vector components are floating-point values.

var componentsPerVector: Int

The number of scalar components in each vector.

var bytesPerComponent: Int

The size, in bytes, of each vector component.

var dataOffset: Int

The offset, in bytes, from the beginning of the data to the first vector component to be used in the geometry source.

