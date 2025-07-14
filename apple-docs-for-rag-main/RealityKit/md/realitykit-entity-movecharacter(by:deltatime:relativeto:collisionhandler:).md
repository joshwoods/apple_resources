

- RealityKit
- Entity
-  moveCharacter(by:deltaTime:relativeTo:collisionHandler:) 

Instance Method

# moveCharacter(by:deltaTime:relativeTo:collisionHandler:)

Moves the character along a specified vector over a period of time.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@discardableResult @MainActor @preconcurrency
func moveCharacter(
    by moveDelta: SIMD3,
    deltaTime: Float,
    relativeTo referenceEntity: Entity?,
    collisionHandler: ((CharacterControllerComponent.Collision) -> Void)? = nil
) -> CharacterControllerComponent.CollisionFlags
```

## Parameters 

`moveDelta`  

Delta vector to attempt to move capsule in collision world.

`deltaTime`  

Time between last frame and current.

`referenceEntity`  

Reference entity that defines the frame of reference of the move delta. Can be `nil`, which is equivalent to “world space”.

`collisionHandler`  

Optional callback when an entity was hit. One call per each hit entity.

## Return Value

Collision flags that indicate the location of the collision.

## Discussion

Moves the character in the collision world, with continuous collision checking and response. This will create character collision events. Entity.transform will be updated on the next engine tick. Use `CharacterControllerStateComponent` to get additional information about the state of the character after the move.

## See Also

### Animating and controlling characters

var characterController: CharacterControllerComponent?

The character controller component for the entity.

var characterControllerState: CharacterControllerStateComponent?

The character controller state for the entity.

func teleportCharacter(to: SIMD3&lt;Float>, relativeTo: Entity?)

Moves the character instantly to a new position.

