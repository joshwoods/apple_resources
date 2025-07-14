

- RealityKit
- AnchorEntity
-  init(world:) 

Initializer

# init(world:)

Creates an anchor entity with a target fixed at the given position in the scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
convenience init(world transform: float4x4)
```

## Parameters 

`transform`  

The transform with which to initialize the world target.

## See Also

### Creating an anchor

init()

Creates a new anchor entity.

convenience init(any Anchor)

init(AnchoringComponent.Target)

Creates an anchor entity targeting a particular kind of anchor.

convenience init(AnchoringComponent.Target, trackingMode: AnchoringComponent.TrackingMode)

convenience init(AnchoringComponent.Target, trackingMode: AnchoringComponent.TrackingMode, physicsSimulation: AnchoringComponent.PhysicsSimulation)

convenience init(anchor: ARAnchor)

Creates an anchor entity that uses an existing AR anchor.

convenience init(plane: AnchoringComponent.Target.Alignment, classification: AnchoringComponent.Target.Classification, minimumBounds: SIMD2&lt;Float>)

Creates an anchor entity that targets a plane with the given characteristics.

convenience init(raycastResult: ARRaycastResult)

Creates an anchor entity using the information about a real-world surface discovered using a ray-cast query.

convenience init(world: SIMD3&lt;Float>)

Creates an anchor entity with a target fixed at the given position in the scene.

