

- RealityKit
- CharacterControllerComponent
-  CharacterControllerComponent.Collision 

Structure

# CharacterControllerComponent.Collision

A container that holds collision state for the character controller.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct Collision
```

## Overview

All coordinates are in *physics space*, the coordinate system of the physics simulation.

## Topics

### Initializers

init(characterEntity: Entity, hitEntity: Entity, hitPosition: SIMD3&lt;Float>, hitNormal: SIMD3&lt;Float>, moveDirection: SIMD3&lt;Float>, moveDistance: Float)

Create Collision and initialize all fields.

### Instance Properties

var characterEntity: Entity

Entity owning the character controller component.

var hitEntity: Entity

The entity that was hit by the character controller.

var hitNormal: SIMD3&lt;Float>

Hit normal relative to physics origin. In physics space.

var hitPosition: SIMD3&lt;Float>

Hit position relative to physics origin. In physics space.

var moveDirection: SIMD3&lt;Float>

Move direction controller was moving (unit vector). In physics space.

var moveDistance: Float

Move distance controller was attempting to move. In physics space.

## See Also

### Character control

struct CharacterControllerComponent

A component that manages character movement.

struct CollisionFlags

An option set that specifies which parts of the character capsule have collided with other objects.

struct CharacterControllerStateComponent

A component that represents the state of a character controller.

