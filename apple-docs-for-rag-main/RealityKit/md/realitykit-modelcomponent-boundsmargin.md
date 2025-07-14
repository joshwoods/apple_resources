

- RealityKit
- ModelComponent
-  boundsMargin 

Instance Property

# boundsMargin

A margin applied to an entity’s bounding box that determines object visibility.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var boundsMargin: Float { get set }
```

## Mentioned in 

Modifying RealityKit rendering using custom materials

## Discussion

When determining which entities are currently visible, RealityKit tests each entity’s bounding box to see if it overlaps with the camera’s field of view (also known as the camera’s *frustum*). For efficiency, entities with a bounding box that don’t overlap the camera’s frustum aren’t rendered. Use this property to prevent RealityKit from incorrectly culling entities that use a CustomMaterial with a geometry modifier that moves vertices outside of the entity’s bounding box.

RealityKit adds the value of `boundsMargin` to the bounding box before determining which entities are visible.

