

- RealityKit
-  CharacterControllerStateComponent 

Structure

# CharacterControllerStateComponent

A component that represents the state of a character controller.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct CharacterControllerStateComponent
```

## Overview

RealityKit adds this component to an entity when you add a CharacterControllerComponent instance to it. Manually adding this component to an entity that has a character controller component has no effect because it’s redundant.

## Topics

### Creating a state component

init()

### Accessing character controller state

let isOnGround: Bool

A Boolean value that indicates whether the character controller is on the ground.

let velocity: SIMD3&lt;Float>

The linear speed relative to the origin in physics space.

### Default Implementations

Component Implementations

## Relationships

### Conforms To

- Component

## See Also

### Character control

struct CharacterControllerComponent

A component that manages character movement.

struct Collision

A container that holds collision state for the character controller.

struct CollisionFlags

An option set that specifies which parts of the character capsule have collided with other objects.

