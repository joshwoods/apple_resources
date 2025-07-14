

- SceneKit
- SCNGeometrySource
-  init(data:semantic:vectorCount:usesFloatComponents:componentsPerVector:bytesPerComponent:dataOffset:dataStride:) 

Initializer

# init(data:semantic:vectorCount:usesFloatComponents:componentsPerVector:bytesPerComponent:dataOffset:dataStride:)

Creates a geometry source from the specified data and options.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
convenience init(
    data: Data,
    semantic: SCNGeometrySource.Semantic,
    vectorCount: Int,
    usesFloatComponents floatComponents: Bool,
    componentsPerVector: Int,
    bytesPerComponent: Int,
    dataOffset offset: Int,
    dataStride stride: Int
)
```

## Parameters 

`data`  

The data for the geometry source.

`semantic`  

The semantic value (or attribute) that the geometry source describes for each vertex. See Geometry Semantic Identifiers for available values.

`vectorCount`  

The number of geometry source vectors.

`floatComponents`  

A Boolean value that indicates whether vector components are floating-point values. Specify true for floating-point values, or false for integer values.

`componentsPerVector`  

The number of scalar components in each vector.

`bytesPerComponent`  

The size, in bytes, of each vector component.

`offset`  

The offset, in bytes, from the beginning of the data to the first vector component to be used in the geometry source.

`stride`  

The number of bytes from each vector to the next in the data.

## Return Value

A new geometry source object.

## Discussion

A geometry source’s data is an array of vectors, each of which represents a particular attribute (or semantic) of a vertex in the geometry. The other parameters determine how SceneKit interprets this data. For example, an array of vertex positions may have three 32-bit floating-point components per vector, but an array of texture coordinates may have two 8-bit integer coponents per vector. You can use the `offset` and `stride` parameters together to interleave data for multiple geometry sources in the same array, improving rendering performance. See SCNGeometrySource for details.

To create a custom SCNGeometry object from the geometry source, use the init(sources:elements:) method.

## See Also

### Creating Geometry Sources

convenience init(vertices: [SCNVector3])

Creates a geometry source from an array of vertex positions.

convenience init(normals: [SCNVector3])

Creates a geometry source from an array of normal vectors.

convenience init(textureCoordinates: [CGPoint])

Creates a geometry source from an array of texture coordinate points.

