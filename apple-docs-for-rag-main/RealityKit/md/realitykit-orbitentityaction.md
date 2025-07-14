

- RealityKit
-  OrbitEntityAction 

Structure

# OrbitEntityAction

An action which animates the transform of an entity to revolve around a specified pivot entity.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct OrbitEntityAction
```

## Overview

This action moves an entity in a circular path by gradually adjusting its local transform. The animation starts from the entity’s initial transform, and rotates around the pivot entity. The orbitalAxis specifies which cartesian axis to rotate around in world space.. The axis is resolved when the action starts to produce an axis of rotation around the pivot entity. The full orbit completes after the action has ended.

The example below creates an animation that orbits an entity around the x-axis two times for five seconds.

```
// Create an action entity resolution to the pivot entity 
// that exists in the scene.
let pivotEntity: ActionEntityResolution = .entityNamed("pivotEntity")

// Create an action that performs an orbit around the 
// specified pivot entity.
let orbitEntityAction = OrbitEntityAction(pivotEntity: pivotEntity,
                                          revolutions: 2,
                                          orbitalAxis: [0, 1, 0],
                                          isOrientedToPath: true,
                                          isAdditive: false)

// A five second animation that plays an animation causing the entity to
// orbit around the pivot.
let orbitAnimation = try AnimationResource
    .makeActionAnimation(for: orbitEntityAction,
                         duration: 5.0,
                         bindTarget: .transform)

// Play the five second orbit animation.
entity.playAnimation(orbitAnimation)
```

Note

Use the orbitalAxis to determine whether the entity orbits clockwise or counterclockwise.

Important

This action directly animates the BindTarget.transform on the bound entity. Ensure a correct bind target is supplied when creating the animation.

Important

For a successful orbit, ensure the translational offset between the target and pivot entity are not parallel to the orbit axis.

## Topics

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

init(pivotEntity: ActionEntityResolution, revolutions: Float, orbitalAxis: SIMD3&lt;Float>, isOrientedToPath: Bool, isAdditive: Bool)

Creates a new orbit entity action.

### Instance Properties

var animatedValueType: (any AnimatableData.Type)?

The type for the value that the action modifies over time.

var isAdditive: Bool

A Boolean value that indicates whether the animation system additively blends the action’s output with the base value.

var isOrientedToPath: Bool

A Boolean value that indicates whether the orbiting object updates its orientation during the animation to orient itself along the rotation path.

var orbitalAxis: SIMD3&lt;Float>

A vector that describes the axis of rotation (in world space).

var pivotEntity: ActionEntityResolution

The entity that the target entity orbits around.

var revolutions: Float

The number of rotations to complete before stopping.

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

struct PlayAnimationAction

An action that plays an animation on the given target entity with a range of playback options.

struct PlayAudioAction

An action which plays an audio resource on the given target entity.

struct SetEntityEnabledAction

An action that enables or disables the targeted entity and its descendants when played as an animation.

struct SpinAction

An action which animates the transform of an entity to rotate around a specified local axis.

