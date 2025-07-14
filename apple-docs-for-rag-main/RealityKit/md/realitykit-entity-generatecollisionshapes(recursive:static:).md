

- RealityKit
- Entity
-  generateCollisionShapes(recursive:static:) 

Instance Method

# generateCollisionShapes(recursive:static:)

Creates the shape used to detect collisions between two entities that have collision components.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func generateCollisionShapes(
    recursive: Bool,
    static isStatic: Bool
)
```

## Parameters 

`recursive`  

A Boolean that you set to `true` to also generate the collision shapes for all descendants of the entity.

`isStatic`  

A Boolean value that indicates whether the colliders move. Set this to `true` to indicate the colliders don’t move. Non-moving, static colliders are more efficient to use than non-static ones.

## Discussion

Call this method on entities that adopt the HasModel and HasCollision protocols to prepare a shape used for collision detection. The method stores the shape in the entity’s CollisionComponent instance.

For non-model entities, the method has no effect. Nevertheless, the method is defined for all entities so that you can call it on any entity, and have the calculation propagate recursively to all that entity’s descendants.

## See Also

### Creating a collision shape

func generateCollisionShapes(recursive: Bool)

Creates the shape used to detect collisions between two entities that have collision components.

