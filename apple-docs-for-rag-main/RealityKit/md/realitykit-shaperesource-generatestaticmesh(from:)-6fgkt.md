

- RealityKit
- ShapeResource
-  generateStaticMesh(from:) 

Type Method

# generateStaticMesh(from:)

Creates a static collision mesh from a mesh resource.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
static func generateStaticMesh(from mesh: MeshResource) async throws -> ShapeResource
```

## Parameters 

`mesh`  

The mesh resource for generating the collision shape.

## Discussion

You can use only the physics body mode PhysicsBodyMode.static and the collision component mode CollisionComponent.Mode.default with this shape.

The code example below assumes calling this method from a synchronous block:

```
// Use a low-priority task because generating collision meshes can take a while.
let myShapeTask = Task(priority: .low) {
    let meshResource = await MeshResource(
        shape: .generateBox(size: [5, 5, 5])
    )

    guard let shape = try? await ShapeResource.generateStaticMesh(
        from: meshResource
    ) else { return }

    // You can use the `ShapeResource` to make a
    // `CollisionComponent`, and add that to an entity.
    // Run this from the main thread.
    await MainActor.run {
        let entity = Entity()
        let collision = CollisionComponent(shapes: [shape])
        entity.components.set(collision)

        // Note that you can't set `mode` to `.dynamic`.
        // This only supports `.static`.
        let physicsBody = PhysicsBodyComponent(
            massProperties: .default,
            material: nil,
            mode: .static
        )
        entity.components.set(physicsBody)
        // ...
    }
}
```

