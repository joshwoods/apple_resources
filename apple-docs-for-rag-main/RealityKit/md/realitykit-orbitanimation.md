

- RealityKit
-  OrbitAnimation 

Structure

# OrbitAnimation

An animation that revolves an entity around its origin.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct OrbitAnimation
```

## Overview

This class moves an entity in a circular path by gradually adjusting its local transform. The animation sets the entity’s initial position with startTransform and rotates it around the point `(0,` `0,` `0)`. The axis specifies which cartesian axis around which to rotate. The full orbit completes after duration lapses.

If the target entity contains child entities, the target entity orbits the children.

### Revolve an entity around its origin

The following code creates an animation that orbits an entity around the y-axis 3 times over `6` seconds.

```
let yAxis: SIMD3 = [0, 1, 0]
let startingPosition: SIMD3 = [0.25, 0, 0]

let orbit = OrbitAnimation(
    name: "orbit",
    duration: 6,
    axis: yAxis,
    startTransform: Transform(translation: startingPosition),
    spinClockwise: false,
    orientToPath: true,
    rotationCount: 3,
    bindTarget: .transform
)
```

The newly created animation can be trimmed after creation, to last only 4 seconds.

```
// Create an animation clip that skips the first two seconds.
let trimmed = orbit.trimmed(start: 2)
```

Use generate(with:) to convert `OrbitAnimation` to an AnimationResource that can be applied to your entity with playAnimation(_:transitionDuration:blendLayerOffset:separateAnimatedValue:startsPaused:clock:).

 Video with custom controls. 

 Content description: A screen recording of a red cube in a living room scene. The cube is slightly offset from the center, and rotates around the y-axis twice at a rate of 1 rotation every 2 seconds. 

Play 

## Topics

### Creating an animation

init(name: String, duration: TimeInterval, axis: SIMD3&lt;Float>, startTransform: Transform, spinClockwise: Bool, orientToPath: Bool, rotationCount: Float, bindTarget: BindTarget?, blendLayer: Int32, repeatMode: AnimationRepeatMode, fillMode: AnimationFillMode, isAdditive: Bool, trimStart: TimeInterval?, trimEnd: TimeInterval?, trimDuration: TimeInterval?, offset: TimeInterval, delay: TimeInterval, speed: Float)

Creates an animation that revolves an entity around its origin.

### Configuring the animation

var startTransform: Transform

The pose of the orbiting object at the start of the animation.

var axis: SIMD3&lt;Float>

A 3D vector that points in the direction of the axis around which to rotate.

var name: String

A textual name for the animation.

var bindTarget: BindTarget

A textual name that identifies the particular property that animates.

var blendLayer: Int32

The order in which the framework composites the animation.

var rotationCount: Float

The number of times to rotate the target entity before stopping.

var spinClockwise: Bool

A Boolean value that indicates whether the object orbits the center point in the clockwise direction.

var orientToPath: Bool

A Boolean value that indicates whether the orbiting object updates its orientation during the animation to orient itself along the rotation path.

var additive: Bool

A Boolean value that indicates whether the animation builds on the current state of the target entity or resets the state before running.

### Timing the animation

var speed: Float

A factor that changes the animation’s rate of playback.

var delay: TimeInterval

An amount of time that lapses before the animation plays.

var duration: TimeInterval

The elapsed time for one complete rotation.

var offset: TimeInterval

The time, in seconds, at which the animation begins within the duration.

var trimDuration: TimeInterval?

An optional duration that overrides the calculated duration.

var trimStart: TimeInterval?

The optional time, in seconds, at which the animation plays.

var trimEnd: TimeInterval?

The optional time, in seconds, at which the animation stops.

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

struct AnimationView

An animation that represents a variation of another animation.

protocol AnimationDefinition

The configuration, including target object, timeframe, and visual semantics, of an animation.

struct AnimationFillMode

Options that determine which animation frames display outside of the normal duration.

struct AnimationGroup

A collection of animations that play simultaneously.

struct AnimationHandoffType

The type of handoff the play animation method performs between a current animation and a new animation.

