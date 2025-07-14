

- RealityKit
- AnchorEntity
-  init(plane:classification:minimumBounds:) 

Initializer

# init(plane:classification:minimumBounds:)

Creates an anchor entity that targets a plane with the given characteristics.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
convenience init(
    plane alignment: AnchoringComponent.Target.Alignment,
    classification: AnchoringComponent.Target.Classification = .any,
    minimumBounds: SIMD2 = [0, 0]
)
```

## Parameters 

`alignment`  

The alignment of the plane to target, like horizontal or vertical.

`classification`  

The classification of the target plane to look for, like floor or ceiling.

`minimumBounds`  

The minimum size of the target plane.

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

convenience init(raycastResult: ARRaycastResult)

Creates an anchor entity using the information about a real-world surface discovered using a ray-cast query.

convenience init(world: float4x4)

Creates an anchor entity with a target fixed at the given position in the scene.

convenience init(world: SIMD3&lt;Float>)

Creates an anchor entity with a target fixed at the given position in the scene.

