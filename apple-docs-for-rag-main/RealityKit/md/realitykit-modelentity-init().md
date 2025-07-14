

- RealityKit
- ModelEntity
-  init() 

Initializer

# init()

Creates a model entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
required init()
```

## See Also

### Creating a model

init(mesh: MeshResource, materials: [any Material])

Creates a model entity with a particular mesh and set of materials.

init(mesh: MeshResource, materials: [any Material], collisionShape: ShapeResource, mass: Float)

Creates a model entity with a particular mesh, set of materials, collision shape, and mass.

init(mesh: MeshResource, materials: [any Material], collisionShapes: [ShapeResource], mass: Float)

Creates a model entity with a particular mesh, set of materials, a composite collision shape, and mass.

