

- SceneKit
- SCNGeometrySource
-  usesFloatComponents 

Instance Property

# usesFloatComponents

A Boolean value that indicates whether vector components are floating-point values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var usesFloatComponents: Bool { get }
```

## Discussion

If true, SceneKit interprets the geometry source’s data as an array of vectors whose components are floating-point values. The type of floating-point value is determined by the SCNGeometrySource property: 4 bytes for `float` values or 8 bytes for `double` values.

If false, SceneKit interprets the geometry source’s data as an array of vectors whose components are integer values. The type of integer value is determined by the SCNGeometrySource property; for example, 2 bytes for `unsigned short` values or 4 bytes for `unsigned int` values.

## See Also

### Inspecting a Geometry Source

var data: Data

The data for the geometry source.

var semantic: SCNGeometrySource.Semantic

The semantic value (or attribute) the geometry source describes for each vertex.

var vectorCount: Int

The number of vectors in the data.

var componentsPerVector: Int

The number of scalar components in each vector.

var bytesPerComponent: Int

The size, in bytes, of each vector component.

var dataOffset: Int

The offset, in bytes, from the beginning of the data to the first vector component to be used in the geometry source.

var dataStride: Int

The number of bytes from a vector to the next one in the data.

