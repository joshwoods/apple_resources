

- Model I/O
- MDLTransformComponent
-  globalTransform(with:atTime:) 

Type Method

# globalTransform(with:atTime:)

Returns the absolute coordinate transformation for an object in a transform hierarchy.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
optional static func globalTransform(
    with object: MDLObject,
    atTime time: TimeInterval
) -> matrix_float4x4
```

## Parameters 

`object`  

An object with a transform component.

`time`  

The time sample for which to request information.

## Return Value

The transform matrix that defines a local coordinate space relative to the root coordinate space of the hierarchy containing the object.

## Discussion

Asset file formats typically describe collections of meshes, models, or lights with a hierarchy of transforms relative to the scene containing them all. For example, if you call this method on a MDLMesh object loaded from a MDLAsset instance, Model I/O concatenates the local transformations of the mesh, its parent object, and any further parent objects to return the mesh’s transform relative to the root coordinate space of the scene that the asset describes.

