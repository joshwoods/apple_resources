

- SceneKit
- SCNGeometryElement
-  init(data:primitiveType:primitiveCount:bytesPerIndex:) 

Initializer

# init(data:primitiveType:primitiveCount:bytesPerIndex:)

Creates a geometry element from the specified data and options.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
convenience init(
    data: Data?,
    primitiveType: SCNGeometryPrimitiveType,
    primitiveCount: Int,
    bytesPerIndex: Int
)
```

## Parameters 

`data`  

The data describing the element.

`primitiveType`  

The drawing primitive that connects vertices when rendering the geometry element. For possible values, see SCNGeometryPrimitiveType.

`primitiveCount`  

The number of primitives in the element.

`bytesPerIndex`  

The number of bytes that represent a single index value in the data.

## Return Value

A new geometry element object.

## Discussion

An element’s data is an array of index values identifying vertices in a geometry source. SceneKit interprets the data as an array of unsigned integers (whose size is specified by the `bytesPerIndex` parameter), and then connects the vertices in the order specified by this array, arranged according to the `primitiveType` parameter.

To create a custom SCNGeometry object from the geometry element, use the init(sources:elements:) method.

## See Also

### Creating a Geometry Element

convenience init&lt;IndexType>(indices: [IndexType], primitiveType: SCNGeometryPrimitiveType)

Creates a geometry element from the specified array of index values.

