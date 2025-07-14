

- RealityKit
-  FromToByAction 

Structure

# FromToByAction

An action that starts, stops, or increments by a specific value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct FromToByAction where Value : AnimatableData
```

## Overview

This action animates a bound parameters value over time. Specifying a from value represents the animated properties’ initial value at the start of the animation. Specifying a to determines the value of the property at the end of the animation. Specifying aby adds a value to the properties initial state, which calculates the value at the end of the animation.

This action exposes FromToByAction.TransformMode which is used when animating a Transform property. Use this mode to determine the reference space the property is relative to. For example, FromToByAction.TransformMode.local means the provided transforms are relative to the transform of the bound entity. The only exception is when by is specified, this is relative to the space of the starting transform.

Note

`FromToByAction` doesn’t support JointTransforms or BlendShapeWeights types. Use FromToByAnimation to animate these types.

### Creating a from, to, by action to animate an entity’s opacity

The example below creates an animation which gradually animates the bound entity’s opacity property for five seconds with a linear transition. In this example, the entity starts with opacity at `1.0`.

```
// Create an action that gradually animates a float value
// towards `0.0`, with a linear transition.
//
// This action does not have a `from` value supplied, 
// meaning this starts from the default source value.
let opacityAction = FromToByAction(to: 0.0,
                                          timing: .linear,
                                          isAdditive: false)

// A five second animation that plays an animation causing the entity to
// gradually animate the `.opacity` property towards `0.0`.
//
// This makes the entity fade-out.
let opacityAnimation = try AnimationResource
    .makeActionAnimation(for: opacityAction,
                         duration: 5.0,
                         bindTarget: .opacity)

// Play the five second animation on the entity that will fade-out.
entity.playAnimation(opacityAnimation)
```

### Create a from, to, by action to animate an entity’s transform property

The example below creates an animation which gradually animates the bound entities transform property for five seconds with a linear transition.

```
// Create a transform to start animating from.
let startTransform = Transform(translation: [0.0, 2.0, 0.0])

// Create a transform to animate towards.
let endTransform = Transform(translation: [0.0, -2.0, 0.0])

// Create an action that gradually animates a transform value.
//
// This starts `from` a specified value, and animates towards
// a specified `to` value.
//
// The bound entity will move in the space relative to its parent.
let transformAction = FromToByAction(from: startTransform,
                                                to: endTransform,
                                                mode: .parent,
                                                timing: .linear,
                                                isAdditive: false)

// A five second animation that plays an animation causing 
// the entity to gradually move from a specific start, and end transform
let transformAnimation = try AnimationResource
    .makeActionAnimation(for: transformAction,
                         duration: 5.0,
                         bindTarget: .transform)

// Play the five second animation on the entity that will cause it to move.
entity.playAnimation(transformAnimation)
```

Note

The default source value is the base value of the of animated property. If multiple animations target the property, then the framework observes the output of the previous animation as the subsequent animation’s default source value.

Important

This action animates various bound properties, for example BindTarget.transform on the bound entity. Ensure a correct bind target is supplied when creating the animation.

Note

For more information on the combination of inputs this action supports see FromToByAnimation.

Important

If you do not provide values for any of the `from`, `to`, and `by` parameters, the animation stays at the default source value.

## Topics

### Initializers

init(by: Value, timing: AnimationTimingFunction, isAdditive: Bool)

Creates a new action to animate from the deaultSource by a transform relative to the starting transform.

init(from: Value, by: Value?, mode: FromToByAction&lt;Value>.TransformMode, timing: AnimationTimingFunction, isAdditive: Bool)

Creates a new action that interpolates from a specified starting transform towards a specified transform, which is relative to the start. Alternatively, interpolates towards the default source if `by` is not supplied.

init(from: Value?, by: Value, timing: AnimationTimingFunction, isAdditive: Bool)

Creates a new action that interpolates towards a specified value, which is relative to the starting value.

init(from: Value, timing: AnimationTimingFunction, isAdditive: Bool)

Creates a new from to by action to animate from a specified value, towards the defaultSource value.

init(from: Value?, to: Value, mode: FromToByAction&lt;Value>.TransformMode, timing: AnimationTimingFunction, isAdditive: Bool)

Creates a new action that interpolates towards a specified final transform.

init(from: Value?, to: Value, timing: AnimationTimingFunction, isAdditive: Bool)

Creates a new action that interpolates towards a specified final value.

init(to: Value, by: Value, mode: FromToByAction&lt;Value>.TransformMode, timing: AnimationTimingFunction, isAdditive: Bool)

Creates a action to animate towards a final value. The starting value is determined by adding the inverse of `by` to the specified final value.

init(to: Value, by: Value, timing: AnimationTimingFunction, isAdditive: Bool)

Creates a new from to by action to animate towards a final value. The starting value is determined by adding the inverse of `by` to the specified final value.

### Instance Properties

let animatedValueType: (any AnimatableData.Type)?

The type for the value that the action modifies over time.

let by: Value?

The amount that the animated property changes during the animation.

let from: Value?

The state of the animated property before the animation starts.

var isAdditive: Bool

A Boolean value that indicates whether the animation system additively blends the action’s output with the base value.

let isReversible: Bool

Specifies whether you can play this action in reverse in order to undo prior operations.

var mode: FromToByAction&lt;Transform>.TransformMode?

Determines the entities transform from and to are relative to.

var timingFunction: AnimationTimingFunction

A timing function that controls the progress of the animation.

let to: Value?

The state of the animated property after the animation ends.

### Type Aliases

typealias EventParameterType

The associated event parameter type.

### Enumerations

enum DecodingErrors

enum TransformMode

Options available to determine the space the bound entity should be relative to.

### Default Implementations

Decodable Implementations

Encodable Implementations

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

struct SpinAction

An action which animates the transform of an entity to rotate around a specified local axis.

