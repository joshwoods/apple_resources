

- RealityKit
- Entity
-  characterController 

Instance Property

# characterController

The character controller component for the entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
var characterController: CharacterControllerComponent? { get set }
```

## See Also

### Animating and controlling characters

var characterControllerState: CharacterControllerStateComponent?

The character controller state for the entity.

func moveCharacter(by: SIMD3&lt;Float>, deltaTime: Float, relativeTo: Entity?, collisionHandler: ((CharacterControllerComponent.Collision) -> Void)?) -> CharacterControllerComponent.CollisionFlags

Moves the character along a specified vector over a period of time.

func teleportCharacter(to: SIMD3&lt;Float>, relativeTo: Entity?)

Moves the character instantly to a new position.

