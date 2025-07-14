

- RealityKit
-  ImpulseAction 

Structure

# ImpulseAction

An action that applies an impulse to the physics body at its center of mass when played as an animation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ImpulseAction
```

## Overview

This action requires a CollisionComponent and PhysicsBodyComponent with the mode set to PhysicsBodyMode.dynamic. Without these settings, the impulse has no effect on the entity.

The example below creates an animation which applies an impulse to the entity after five seconds.

```
// Create an action to apply an impulse, forcing the object to move upwards.
let impulseAction = ImpulseAction(linearImpulse: [0, 1, 0])

// Create a small positive duration value.
let duration: TimeInterval = 1 / 30.0

// Create an animation for the action, which will start playing
// after five seconds.
let impulseAnimation = try AnimationResource
    .makeActionAnimation(for: impulseAction,
                         duration: duration,
                         delay: 5.0)

// Play the sequence animation that will play the actions.
entity.playAnimation(impulseAnimation)
```

Important

This action does not directly animate a bound property, such as BindTarget.transform.

Tip

This action performs instantaneously, consider supplying a small positive duration value when creating the animation.

## Topics

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

init(targetEntity: ActionEntityResolution, linearImpulse: SIMD3&lt;Float>)

Creates a new impulse action.

### Instance Properties

var animatedValueType: (any AnimatableData.Type)?

The type for the value that the action modifies over time.

var linearImpulse: SIMD3&lt;Float>

An impulse in newton seconds (in physics simulation space).

var targetEntity: ActionEntityResolution

The entity that the impulse acts upon.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Type Aliases

typealias EventParameterType

The associated event parameter type.

### Default Implementations

EntityAction Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- EntityAction

## See Also

### Built-in actions

struct BillboardAction

An action that animates the blend factor of an entity’s billboard component.

struct EmphasizeAction

An action that performs an animation to call attention to an entity.

struct FromToByAction

An action that starts, stops, or increments by a specific value.

struct OrbitEntityAction

An action which animates the transform of an entity to revolve around a specified pivot entity.

struct PlayAnimationAction

An action that plays an animation on the given target entity with a range of playback options.

struct PlayAudioAction

An action which plays an audio resource on the given target entity.

struct SetEntityEnabledAction

An action that enables or disables the targeted entity and its descendants when played as an animation.

struct SpinAction

An action which animates the transform of an entity to rotate around a specified local axis.

