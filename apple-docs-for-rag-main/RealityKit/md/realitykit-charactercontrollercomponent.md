

- RealityKit
-  CharacterControllerComponent 

Structure

# CharacterControllerComponent

A component that manages character movement.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct CharacterControllerComponent
```

## Overview

To use a character controller, add a `CharacterControllerComponent` to your entity to make it a character entity. Use moveCharacter(by:deltaTime:relativeTo:collisionHandler:) to move your character and respond to collisions, or teleportCharacter(to:relativeTo:) to place your character instantaneously in 3D space.

Note

PhysicsBodyComponent and CollisionComponent are incompatible with `CharacterControllerComponent`, and RealityKit deactivates them if you add them to the same entity.

## Handle collision

Character entities are capsular, and you can specify their height and radius in the component’s initializer. A character’s capsule shape aligns with its upVector so that the top and bottom of the capsule pass through that direction vector.

Although characters don’t have a `CollisionComponent`, they can still interact with colliders. The collision handler in `moveCharacter(by:deltaTime:relativeTo:collisionHandler:)` allows you to respond to collisions with solid colliders in your scene.

```
entity.moveCharacter(by: velocity * deltaTime, deltaTime: deltaTime, relativeTo: nil) {
    event in
    // Your character collided with `event.hitEntity`.
}
```

To handle collisions with colliders that have a mode of CollisionComponent.Mode.trigger, subscribe to the CollisionEvents.Began event for your RealityView. This event doesn’t occur for solid collisions with your character, but RealityKit invokes it when your character enters a trigger. This is useful for collecting coins, claiming checkpoints, activating enemy behavior when your character enters an area, and many other interactions within games.

## Update your character

A common use case for `CharacterControllerComponent` is to control a character in a video game. Video games have update loops where characters and game logic update once each frame, allowing them to respond to player input in real time. `CharacterControllerComponent` works well in such a setup.

To move your character in response to player input, subscribe to PhysicsSimulationEvents.WillSimulate on RealityViewContent for your scene. The event object contains information like the time delta since the last update, and you can treat this callback as the update loop for your game.

Note

You can also use SceneEvents.Update to run code for each frame, but avoid using it to control physics-based motion in your scene.

Read the values from CharacterControllerStateComponent to accumulate forces (such as gravity) and to check whether the character is on the ground. RealityKit calculates isOnGround and velocity only after you call `moveCharacter(by:deltaTime:relativeTo:collisionHandler:)`, so it’s a good idea to call this function at each update.

```
let gravity: SIMD3 = [0, -50, 0]
let jumpSpeed: Float = 10
content.subscribe(to: PhysicsSimulationEvents.WillSimulate.self, on: playerEntity) {
    event in
    let deltaTime: Float = event.deltaTime
    var velocity: SIMD3 = .zero
    var isOnGround: Bool = false

    // RealityKit automatically adds `CharacterControllerStateComponent` after moving the character for the first time.
    if let ccState = playerEntity.components[CharacterControllerStateComponent.self] {
        velocity = ccState.velocity
        isOnGround = ccState.isOnGround
    }

    if !isOnGround {
        // Gravity is a force, so you need to accumulate it for each frame.
        velocity += gravity * deltaTime
    } else if myPlayerInput.jump {
        // Set the character's velocity directly to launch it in the air when the player jumps.
        velocity.y = jumpSpeed
    }

    playerEntity.moveCharacter(by: velocity * deltaTime, deltaTime: deltaTime, relativeTo: nil) {
        event in
        print("playerEntity collided with \(event.hitEntity.name)")
    }
}
```

The following video shows a character entity jumping in response to player input:

 Video with custom controls. 

 Content description: A video of a white capsule jumping on a flat gray plane in response to player input. 

Play 

## Topics

### Creating a character controller component

init()

Creates a character controller component using default values.

init(radius: Float, height: Float, skinWidth: Float, slopeLimit: Float, stepLimit: Float, upVector: SIMD3&lt;Float>, collisionFilter: CollisionFilter)

Creates a character controller component using specified values.

### Configuring a character

var height: Float

The capsule height.

var radius: Float

The capsule radius.

var skinWidth: Float

An added tolerance around the character capsule.

var slopeLimit: Float

The slope limit expressed as a limit angle in radians.

var stepLimit: Float

The maximum obstacle height that the controller can move over.

var upVector: SIMD3&lt;Float>

The y-axis direction relative to the physics origin.

### Managing character collisions

var collisionFilter: CollisionFilter

The character’s collision filter.

### Reading default values

static let defaultHeight: Float

The capsule height value RealityKit applies when you use the default initializer.

static let defaultRadius: Float

The capsule default radius RealityKit applies when you use the default initializer.

static let defaultSkinWidth: Float

The skin width value RealityKit applies when you use the default initializer.

static let defaultSlopeLimit: Float

The slope limit value RealityKit applies when you use the default initializer.

static let defaultStepLimit: Float

The step limit value RealityKit applies when you use the default initializer.

static let defaultUpVector: SIMD3&lt;Float>

The default up vector RealityKit applies when you use the default initializer.

### Animating a character

struct JointTransforms

A set of animatable transform values for joints that collectively represent a single skeletal pose.

### Handling collisions

struct Collision

A container that holds collision state for the character controller.

struct CollisionFlags

An option set that specifies which parts of the character capsule have collided with other objects.

### Default Implementations

Component Implementations

## Relationships

### Conforms To

- Component

## See Also

### Character control

struct Collision

A container that holds collision state for the character controller.

struct CollisionFlags

An option set that specifies which parts of the character capsule have collided with other objects.

struct CharacterControllerStateComponent

A component that represents the state of a character controller.

