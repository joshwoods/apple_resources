

- RealityKit
- AnchorEntity
-  init(\_:) 

Initializer

# init(\_:)

Creates an anchor entity targeting a particular kind of anchor.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
init(_ target: AnchoringComponent.Target)
```

## Parameters 

`target`  

The real world object the anchor should target.

## See Also

### Creating an anchor

init()

Creates a new anchor entity.

convenience init(any Anchor)

convenience init(AnchoringComponent.Target, trackingMode: AnchoringComponent.TrackingMode)

convenience init(AnchoringComponent.Target, trackingMode: AnchoringComponent.TrackingMode, physicsSimulation: AnchoringComponent.PhysicsSimulation)

convenience init(anchor: ARAnchor)

Creates an anchor entity that uses an existing AR anchor.

convenience init(plane: AnchoringComponent.Target.Alignment, classification: AnchoringComponent.Target.Classification, minimumBounds: SIMD2&lt;Float>)

Creates an anchor entity that targets a plane with the given characteristics.

convenience init(raycastResult: ARRaycastResult)

Creates an anchor entity using the information about a real-world surface discovered using a ray-cast query.

convenience init(world: float4x4)

Creates an anchor entity with a target fixed at the given position in the scene.

convenience init(world: SIMD3&lt;Float>)

Creates an anchor entity with a target fixed at the given position in the scene.

