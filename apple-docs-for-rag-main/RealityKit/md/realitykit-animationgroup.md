

- RealityKit
-  AnimationGroup 

Structure

# AnimationGroup

A collection of animations that play simultaneously.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct AnimationGroup
```

## Overview

This structure concurrently starts the animations it contains. Use a group to:

- Animate more than one property at once.

- Animate the same property at different times.

### Animate multiple properties concurrently

For each animatable property your animation needs to control, create a group and add an animation to the array argument of the initializer. The following listing begins coding an animation group that colorizes 3D numbers that count down over a 4-second duration.

```
let frames: [Float] = [3.0, 2.0, 1.0, 0.0]
let duration = TimeInterval(frames.count)
let anim1 = FromToByAnimation(name: "colorize", from: 0.0, to: 1.0,
    duration: duration, bindTarget: .parameter("foo"))
let anim2 = SampledAnimation(frames: frames, name: "count down",
    frameInterval: duration / frames.count, bindTarget: .parameter("bar"))
let group = AnimationGroup(group: [anim1, anim2], name: "group")
```

### Create a sequence for the same animation

You can play the same animation at different times by grouping multiple AnimationDefinition objects that refer to the same animated property. To disperse their playback at runtime, give each definition a unique delay.

Important

The framework processes animations with a lower blendLayer first, and if the blendLayer matches, in the order in which they appear in the groups array. If two animations on the same property overlap durations at runtime, the one that the framework processes second overwrites the first.

## Topics

### Creating an animation group

init(group: [any AnimationDefinition], name: String, repeatMode: AnimationRepeatMode, fillMode: AnimationFillMode, trimStart: TimeInterval?, trimEnd: TimeInterval?, trimDuration: TimeInterval?, offset: TimeInterval, delay: TimeInterval, speed: Float)

Creates a collection of animations that play simultaneously.

### Configuring the group

var group: [any AnimationDefinition]

A collection of animations to run.

var name: String

A textual name for the group.

var bindTarget: BindTarget

A textual name that refers to a property on which to run the grouped animations.

var blendLayer: Int32

The order in which the framework composites the animation.

var additive: Bool

A Boolean value that indicates whether the animation builds on the current state of the target entity or resets the state before running.

var group_: [any AnimationDefinition]?

An optional collection of animations to run.

Deprecated

### Timing the group

var speed: Float

A factor that increases or decreases the animation’s rate of playback.

var delay: TimeInterval

An amount of time that lapses before the animation plays.

var duration: TimeInterval

The total playback time of the animation.

var offset: TimeInterval

The time, in seconds, at which the animations begin within the duration.

var trimDuration: TimeInterval?

An optional duration that overrides the calculated duration.

var trimStart: TimeInterval?

The time, in seconds, at which the animations play.

var trimEnd: TimeInterval?

The time, in seconds, at which the animations stop.

func trimmed(start: TimeInterval?, end: TimeInterval?, duration: TimeInterval?) -> Self

Edits the animation duration according to the specified time.

### Repeating group playback

var repeatMode: AnimationRepeatMode

An option that determines how the animations repeat.

var fillMode: AnimationFillMode

An option that determines which data displays outside of the normal duration.

func repeated(count: TimeInterval) -> Self

Repeats an animation the number of times specified by an irrational number.

func repeated(count: Int) -> Self

Repeats an animation the number of times specified by a whole number.

func repeatingForever() -> Self

Repeats the animation infinitely.

### Default Implementations

AnimationDefinition Implementations

## Relationships

### Conforms To

- AnimationDefinition

## See Also

### Animation definitions

struct SampledAnimation

An animation that cycles through a series of frames at a constant interval.

enum TweenMode

Options that determine whether an animation switches between frames gradually or abruptly.

struct FromToByAnimation

An animation that starts, stops, or increments by a specific value.

struct AnimationTimingFunction

The pacing of an animation transition.

struct AnimationView

An animation that represents a variation of another animation.

struct OrbitAnimation

An animation that revolves an entity around its origin.

protocol AnimationDefinition

The configuration, including target object, timeframe, and visual semantics, of an animation.

struct AnimationFillMode

Options that determine which animation frames display outside of the normal duration.

struct AnimationHandoffType

The type of handoff the play animation method performs between a current animation and a new animation.

