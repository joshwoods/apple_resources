

- RealityKit
-  SetEntityEnabledAction 

Structure

# SetEntityEnabledAction

An action that enables or disables the targeted entity and its descendants when played as an animation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct SetEntityEnabledAction
```

## Overview

This action toggles the targetEntity isEnabled flag. Use the animation generated from this action within an animation group to determine when the entity should be enabled, and visible in the scene.

The example below creates an animation which disables the entity after five seconds. In this example, the target entity starts enabled.

```
// Create an action entity resolution.
//
// The animation will be played from the parent entity.
let childEntity: ActionEntityResolution = .entityNamed("childEntity")

// Create an action to disable the entity.
let disableEntityAction = SetEntityEnabledAction(targetEntity: childEntity,
                                                 isEnabled: false)

// Create a small positive duration value.
let duration: TimeInterval = 1 / 30.0

// Create an animation to disable the target entity.
let disableEntityAnimation = try AnimationResource
    .makeActionAnimation(for: disableEntityAction,
                         duration: duration,
                         delay: 5.0)

// Play the sequence animation that plays the actions.
rootEntity.playAnimation(disableEntityAnimation)
```

 Video with custom controls. 

 Content description: A screen recording of a red cube in a living room scene. At the start, the cube is visibly enabled in the scene. After some time, the cube is disabled; it's no longer visible in the scene. 

Play 

Note

Animations do not play on entities that are disabled. In order to disable, and enable the target entity, play this action on another entity, such as a root entity, or its parent.

Important

This action does not animate a bound property, such as BindTarget.transform.

Tip

This action performs instantaneously, consider supplying a small positive duration value when creating the animation.

## Topics

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

init(targetEntity: ActionEntityResolution, isEnabled: Bool)

Creates a new set entity enabled action.

### Instance Properties

var animatedValueType: (any AnimatableData.Type)?

The type for the value that the action modifies over time.

var isEnabled: Bool

A Boolean that you set to enable or disable the entity and its descendants.

var targetEntity: ActionEntityResolution

The entity to disable or enable.

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

struct SpinAction

An action which animates the transform of an entity to rotate around a specified local axis.

