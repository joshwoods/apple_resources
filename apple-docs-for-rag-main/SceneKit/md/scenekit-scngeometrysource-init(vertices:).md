

- SceneKit
- SCNGeometrySource
-  init(vertices:) 

Initializer

# init(vertices:)

Creates a geometry source from an array of vertex positions.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.8+tvOSvisionOSwatchOS

``` source
@nonobjc
convenience init(vertices: [SCNVector3])
```

## Parameters 

`vertices`  

An array of three-component vectors, each of which represents a vertex position for the geometry source.

## Return Value

A new geometry source whose semantic property is vertex.

## Discussion

SceneKit converts this data to its own format to optimize rendering performance. To read the converted data, examine the properties of the created SCNGeometrySource object.

To create a custom SCNGeometry object from the geometry source, use the init(sources:elements:) method.

## See Also

### Creating Geometry Sources

convenience init(data: Data, semantic: SCNGeometrySource.Semantic, vectorCount: Int, usesFloatComponents: Bool, componentsPerVector: Int, bytesPerComponent: Int, dataOffset: Int, dataStride: Int)

Creates a geometry source from the specified data and options.

convenience init(normals: [SCNVector3])

Creates a geometry source from an array of normal vectors.

convenience init(textureCoordinates: [CGPoint])

Creates a geometry source from an array of texture coordinate points.

