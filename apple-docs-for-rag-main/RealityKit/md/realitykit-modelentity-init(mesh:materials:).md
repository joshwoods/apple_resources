

- RealityKit
- ModelEntity
-  init(mesh:materials:) 

Initializer

# init(mesh:materials:)

Creates a model entity with a particular mesh and set of materials.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
init(
    mesh: MeshResource,
    materials: [any Material] = []
)
```

## Parameters 

`mesh`  

A mesh that defines the geometry of the model.

`materials`  

Material resources that define the appearance of the model.

## See Also

### Creating a model

init()

Creates a model entity.

init(mesh: MeshResource, materials: [any Material], collisionShape: ShapeResource, mass: Float)

Creates a model entity with a particular mesh, set of materials, collision shape, and mass.

init(mesh: MeshResource, materials: [any Material], collisionShapes: [ShapeResource], mass: Float)

Creates a model entity with a particular mesh, set of materials, a composite collision shape, and mass.

