

- RealityKit
-  SpinAction 

Structure

# SpinAction

An action which animates the transform of an entity to rotate around a specified local axis.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct SpinAction
```

## Overview

This action rotates an entity around itself from a specified localAxis gradually adjusting its local transform. The localAxis specifies which cartesian axis around which to rotate in local space. The full spin completes after the action has ended.

The example below creates an animation that spins an entity around the x-axis two times for five seconds with a linear transition.

```
// Create an action that performs a spin around the specified local axis
// with a linear transition.
let spinAction = SpinAction(revolutions: 2,
                            localAxis: [1, 0, 0],
                            timingFunction: .linear,
                            isAdditive: false)

// A five second animation that plays an animation causing the entity to
// spin around a specified local axis.
let spinAnimation = try AnimationResource
    .makeActionAnimation(for: spinAction,
                         duration: 5.0,
                         bindTarget: .transform)

// Play the five second spin animation.
entity.playAnimation(spinAnimation)
```

Note

Use the localAxis to determine whether the entity spins clockwise or counterclockwise.

Important

This action directly animates the BindTarget.transform on the bound entity. Ensure a correct bind target is supplied when creating the animation.

## Topics

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

init(revolutions: Float, localAxis: SIMD3&lt;Float>, timingFunction: AnimationTimingFunction, isAdditive: Bool)

Creates a new spin action.

### Instance Properties

var animatedValueType: (any AnimatableData.Type)?

The type for the value that the action modifies over time.

var isAdditive: Bool

A Boolean value that indicates whether the animation system additively blends the action’s output with the base value.

var localAxis: SIMD3&lt;Float>

A vector that describes the axis of rotation (in local space).

var revolutions: Float

The number of rotations to complete before stopping.

var timingFunction: AnimationTimingFunction

A timing function that controls the progress of the animation.

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

struct ImpulseAction

An action that applies an impulse to the physics body at its center of mass when played as an animation.

struct OrbitEntityAction

An action which animates the transform of an entity to revolve around a specified pivot entity.

struct PlayAnimationAction

An action that plays an animation on the given target entity with a range of playback options.

struct PlayAudioAction

An action which plays an audio resource on the given target entity.

struct SetEntityEnabledAction

An action that enables or disables the targeted entity and its descendants when played as an animation.

