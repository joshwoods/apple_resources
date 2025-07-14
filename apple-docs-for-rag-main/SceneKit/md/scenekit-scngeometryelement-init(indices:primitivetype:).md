

- SceneKit
- SCNGeometryElement
-  init(indices:primitiveType:) 

Initializer

# init(indices:primitiveType:)

Creates a geometry element from the specified array of index values.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.8+tvOSvisionOSwatchOS

``` source
convenience init(
    indices: [IndexType],
    primitiveType: SCNGeometryPrimitiveType
) where IndexType : FixedWidthInteger
```

## Parameters 

`indices`  

An array of index values, each of which identifies a vertex in a geometry source.

`primitiveType`  

The drawing primitive that connects vertices when rendering the geometry element. For possible values, see SCNGeometryPrimitiveType.

## Discussion

SceneKit connects the vertices in the order specified by the `indices` array, arranged according to the `primitiveType` parameter.This initializer is equivalent to the init(data:primitiveType:primitiveCount:bytesPerIndex:) initializer, but does not require an intermediary Data object; instead, it automatically infers the necessary allocation size and bytesPerIndex values based on the contents of the `indices` array.

To create a custom SCNGeometry object from the geometry element, use the init(sources:elements:) initializer.

## See Also

### Creating a Geometry Element

convenience init(data: Data?, primitiveType: SCNGeometryPrimitiveType, primitiveCount: Int, bytesPerIndex: Int)

Creates a geometry element from the specified data and options.

