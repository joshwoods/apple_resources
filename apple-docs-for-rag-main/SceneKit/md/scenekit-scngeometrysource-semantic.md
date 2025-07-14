

- SceneKit
- SCNGeometrySource
-  semantic 

Instance Property

# semantic

The semantic value (or attribute) the geometry source describes for each vertex.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var semantic: SCNGeometrySource.Semantic { get }
```

## Discussion

A semantic describes an attribute for each vertex, such as position, color, surface normal vector, or texture coordinates.

See SCNGeometrySource.Semantic for available values.

## See Also

### Inspecting a Geometry Source

var data: Data

The data for the geometry source.

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

