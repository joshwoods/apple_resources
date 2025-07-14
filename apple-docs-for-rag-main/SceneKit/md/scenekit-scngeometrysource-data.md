

- SceneKit
- SCNGeometrySource
-  data 

Instance Property

# data

The data for the geometry source.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var data: Data { get }
```

## Discussion

A geometry source’s data is an array of vectors, each of which represents a particular attribute (or semantic) of a vertex in the geometry. The other properties of the geometry source determine how SceneKit interprets this data. For example, an array of vertex positions may have three 32-bit floating-point components per vector, but an array of texture coordinates may have two 8-bit integer coponents per vector.

## See Also

### Inspecting a Geometry Source

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

var dataStride: Int

The number of bytes from a vector to the next one in the data.

