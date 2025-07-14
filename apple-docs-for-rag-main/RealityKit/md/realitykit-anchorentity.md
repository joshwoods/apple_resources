

- RealityKit
-  AnchorEntity 

Class

# AnchorEntity

An anchor that tethers entities to a scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
class AnchorEntity
```

## Mentioned in 

Taking Control of Scene Anchoring

Handling different-sized objects in physics simulations

Adding procedural assets to a scene

Loading entities from a file

## Overview

Control how RealityKit places virtual objects into your scene with anchor entities. `AnchorEntity` conforms to the HasAnchoring protocol, which gives it an AnchoringComponent instance.

RealityKit places anchors based on the anchoring component’s target property. For example, you can configure an anchor entity to rest on a horizontal surface that RealityKit detects in an AR scene like a table or floor, and RealityKit automatically places that anchor after it detects an appropriate horizontal plane in the real world. The example below creates an anchor to a horizontal surface:

```
AnchorEntity(.plane(.horizontal,
                    classification: .any,
                    minimumBounds: SIMD2(0.2, 0.2)
))
```

See Selecting an anchor for a Reality Composer scene for more information about the different types of anchors available when using Reality Composer Pro.

Add anchor entities directly to your scene’s anchors collection, or anywhere else in the scene hierarchy by adding them to the children collection of another entity in your scene. Because `AnchorEntity` is a subclass of Entity, you can make an anchor entity a subentity of any other entity. RealityKit might move anchor entities as the scene updates, so the location and rotation of the anchor entity can change relative to its container entity, even if your code never modifies its transform property.

Some anchor entities might not show up in your scene at all if RealityKit fails to detect an appropriate place for them. For example, an anchor entity with an `image` target doesn’t show up in the scene until RealityKit detects the specified image in the real world.

You can have multiple anchors in a RealityKit scene. For example, one anchor can place a toy car on a horizontal surface, like a table, and another can tie an informative text bubble to an image in the same scene.

Note

By default, physics bodies and colliders affect only entities that share the same anchor.

An entity and its descendants can participate in the physics simulation at the root of your scene by setting its physicsSimulation to AnchoringComponent.PhysicsSimulation.none.

## Topics

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

convenience init(world: float4x4)

Creates an anchor entity with a target fixed at the given position in the scene.

convenience init(world: SIMD3&lt;Float>)

Creates an anchor entity with a target fixed at the given position in the scene.

### Configuring the anchor

var anchoring: AnchoringComponent

The component that describes how the virtual content is anchored to the real world.

var anchorIdentifier: UUID?

The identifier of the AR anchor with which the anchor entity is associated, or `nil` if it isn’t currently anchored.

func reanchor(AnchoringComponent.Target, preservingWorldTransform: Bool)

Changes the entity’s anchoring, preserving either the world transform or the local transform.

### Default Implementations

HasAnchoring Implementations

## Relationships

### Inherits From

- Entity

### Conforms To

- CustomDebugStringConvertible
- Equatable
- EventSource
- HasAnchoring
- HasHierarchy
- HasSynchronization
- HasTransform
- Hashable
- Identifiable
- RealityCoordinateSpace
- Sendable

## See Also

### Anchoring component

struct AnchoringComponent

A component that anchors virtual content to a real world target.

enum Target

Defines the kinds of real world objects to which an anchor entity can be tethered.

struct TrackingMode

Decides how the `Entity` tracks its target anchor.

protocol HasAnchoring

An interface that enables anchoring of virtual content to a real-world object in an AR scene.

