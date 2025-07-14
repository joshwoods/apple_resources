

- ARKit
- ARSCNFaceGeometry
-  init(device:) 

Initializer

# init(device:)

Creates a SceneKit face geometry for rendering with the specified Metal device object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
convenience init?(device: any MTLDevice)
```

## Parameters 

`device`  

The Metal device to use for rendering the geometry.

## Return Value

A new SceneKit face geometry, or `nil` if the Metal device is unavailable or ARKit face tracking is not supported on the current device.

## Discussion

A newly created ARSCNFaceGeometry instance represents a neutral, generic face; use the update(from:) method to deform the geometry to match a specific facial expression or face shape.

The geometry contains a single geometry element; as such, assigning more than one material has no visible effect (see the inherited materials property).

Calling this initializer is equivalent to calling the init(device:fillMesh:) initializer and passing false for the `fillMesh` parameter.

## See Also

### Creating a Geometry

convenience init?(device: any MTLDevice, fillMesh: Bool)

Creates a SceneKit face geometry, optionally filling in gaps in the mesh for the eyes and mouth.

