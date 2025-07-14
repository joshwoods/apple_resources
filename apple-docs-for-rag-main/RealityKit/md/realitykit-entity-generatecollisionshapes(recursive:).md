

- RealityKit
- Entity
-  generateCollisionShapes(recursive:) 

Instance Method

# generateCollisionShapes(recursive:)

Creates the shape used to detect collisions between two entities that have collision components.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func generateCollisionShapes(recursive: Bool)
```

## Parameters 

`recursive`  

A Boolean that you set to `true` to also generate the collision shapes for all descendants of the entity.

## Mentioned in 

Reducing CPU Utilization in Your RealityKit App

## Discussion

Call this method on entities that adopt the HasModel and HasCollision protocols to prepare a shape used for collision detection. The method stores the shape in the entity’s CollisionComponent instance.

For non-model entities, the method has no effect. Nevertheless, the method is defined for all entities so that you can call it on any entity, and have the calculation propagate recursively to all that entity’s descendants.

## See Also

### Creating a collision shape

func generateCollisionShapes(recursive: Bool, static: Bool)

Creates the shape used to detect collisions between two entities that have collision components.

