

- RealityKit
-  AnimationView 

Structure

# AnimationView

An animation that represents a variation of another animation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct AnimationView
```

## Overview

This structure creates a variation of an existing animation by overriding its configuration. The term *view* in the name signifies that the variation represents a new visual perspective of the existing animation.

### Create a clip of an animation

By supplying a new beginning time (trimStart) and ending time (trimEnd), the following code creates a shorter clip of an existing animation. With trimStart set to `1.0` and trimEnd at `2.0`, the clip spans a one-second duration.

```
// Create or access an existing animation.
let anim1 = FromToByAnimation(name: "Anim1",
    from: 100.0, to: 200.0, duration: 10.0)

// Use a view to create a clip of the original animation.
let view = AnimationView(source: anim1,
    name: "clip",
    bindTarget: nil,
    blendLayer: 0,
    repeatMode: .autoReverse,
    fillMode: [],
    trimStart: 1.0,
    trimEnd: 2.0,
    trimDuration: nil,
    offset: 0,
    delay: 0,
    speed: 1.0)

// Create an animation resource from the clip.
clipResource = try? AnimationResource.generate(with: view)

// Play the clip.
myModelEntity.playAnimation(clipResource)
```

### Define a view in relation to the animation source

The source animation’s timing properties define a *timeline* on which the trimDuration, delay, and speed properties operate to derive the view. The trimDuration property specifies which animation data the view displays. If trimDuration exceeds the length of the source animation’s timeline, the animation plays according to the characteristics of repeatMode. The delay property defines a waiting period before the animation begins, and the speed determines how fast the view plays in relation to the original pace.

## Topics

### Creating an animation view

init(source: any AnimationDefinition, name: String, bindTarget: BindTarget?, blendLayer: Int32, repeatMode: AnimationRepeatMode, fillMode: AnimationFillMode, trimStart: TimeInterval?, trimEnd: TimeInterval?, trimDuration: TimeInterval?, offset: TimeInterval, delay: TimeInterval, speed: Float)

Creates a variation of the given animation by overriding its properties.

### Configuring the animation view

var source: (any AnimationDefinition)?

The original animation that this structure modifies.

var name: String

A textual name for the animation.

var bindTarget: BindTarget

A textual name that identifies the animated property.

var blendLayer: Int32

The order in which the framework composites the animation.

### Timing the animation

var speed: Float

A factor that increases or decreases the animation’s rate of playback.

var delay: TimeInterval

An amount of time that lapses before the animation plays.

var duration: TimeInterval

The total playback time of the animation.

var offset: TimeInterval

The time, in seconds, at which the animation begins within the duration.

var trimDuration: TimeInterval?

An optional duration that overrides the calculated duration.

var trimStart: TimeInterval?

The time, in seconds, at which the source animation plays.

var trimEnd: TimeInterval?

The time, in seconds, at which the source animation stops.

func trimmed(start: TimeInterval?, end: TimeInterval?, duration: TimeInterval?) -> Self

Edits the animation duration according to the specified time.

### Repeating animation playback

var repeatMode: AnimationRepeatMode

An option that determines how the animation repeats.

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

struct OrbitAnimation

An animation that revolves an entity around its origin.

protocol AnimationDefinition

The configuration, including target object, timeframe, and visual semantics, of an animation.

struct AnimationFillMode

Options that determine which animation frames display outside of the normal duration.

struct AnimationGroup

A collection of animations that play simultaneously.

struct AnimationHandoffType

The type of handoff the play animation method performs between a current animation and a new animation.

