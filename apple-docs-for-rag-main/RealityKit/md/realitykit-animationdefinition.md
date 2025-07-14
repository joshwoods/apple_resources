

- RealityKit
-  AnimationDefinition 

Protocol

# AnimationDefinition

The configuration, including target object, timeframe, and visual semantics, of an animation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
protocol AnimationDefinition
```

## Overview

The framework adopts this protocol for several concrete animation objects, such as FromToByAnimation, SampledAnimation, OrbitAnimation, BlendTreeAnimation, AnimationView, and AnimationGroup.

## Topics

### Configuring the animation

var name: String

A textual name for the animation.

**Required**

var bindTarget: BindTarget

A textual name that identifies the particular property that animates.

**Required**

var blendLayer: Int32

The order in which the framework composites the animation.

**Required**

### Timing the animation

var speed: Float

A factor that increases or decreases the animation’s rate of playback.

**Required**

var delay: TimeInterval

An amount of time that elapses before the animation plays.

**Required**

var duration: TimeInterval

The total playback time of the animation.

**Required**

var offset: TimeInterval

The time, in seconds, at which the animation begins within the duration.

**Required**

var trimDuration: TimeInterval?

An optional duration that overrides the source animation’s duration.

**Required**

var trimStart: TimeInterval?

The time, in seconds, at which the animation plays.

**Required**

var trimEnd: TimeInterval?

The time, in seconds, at which the source animation stops.

**Required**

func trimmed(start: TimeInterval?, end: TimeInterval?, duration: TimeInterval?) -> Self

Edits the animation duration according to the specified time.

### Repeating animation playback

var repeatMode: AnimationRepeatMode

An option that determines how the animation repeats.

**Required**

var fillMode: AnimationFillMode

An option that determines which data displays outside of the normal duration.

**Required**

func repeated(count: TimeInterval) -> Self

Repeats an animation the number of times specified by an irrational number.

func repeated(count: Int) -> Self

Repeats an animation the number of times specified by a whole number.

func repeatingForever() -> Self

Repeats the animation infinitely.

## Relationships

### Conforming Types

- ActionAnimation
- AnimationGroup
- AnimationView
- BlendTreeAnimation
- FromToByAnimation
- OrbitAnimation
- SampledAnimation

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

struct AnimationFillMode

Options that determine which animation frames display outside of the normal duration.

struct AnimationGroup

A collection of animations that play simultaneously.

struct AnimationHandoffType

The type of handoff the play animation method performs between a current animation and a new animation.

