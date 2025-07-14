

- RealityKit
- Entity
-  teleportCharacter(to:relativeTo:) 

Instance Method

# teleportCharacter(to:relativeTo:)

Moves the character instantly to a new position.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
func teleportCharacter(
    to position: SIMD3,
    relativeTo referenceEntity: Entity?
)
```

## Parameters 

`position`  

The position to move the character to, relative to `referenceEntity`.

`referenceEntity`  

The entity that defines a frame of reference. Set this to `nil` to indicate world space.

## Discussion

This method moves the character to a location specified relative to another entity. Pass `nil` in `relativeTo` to specify a position in world coordinates. A teleport move happens instantly. RealityKit does no collision checking when it moves the entity.

## See Also

### Animating and controlling characters

var characterController: CharacterControllerComponent?

The character controller component for the entity.

var characterControllerState: CharacterControllerStateComponent?

The character controller state for the entity.

func moveCharacter(by: SIMD3&lt;Float>, deltaTime: Float, relativeTo: Entity?, collisionHandler: ((CharacterControllerComponent.Collision) -> Void)?) -> CharacterControllerComponent.CollisionFlags

Moves the character along a specified vector over a period of time.

