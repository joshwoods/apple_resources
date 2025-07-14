

- RealityKit
-  SampledAnimation 

Structure

# SampledAnimation

An animation that cycles through a series of frames at a constant interval.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct SampledAnimation where Value : AnimatableData
```

## Overview

To specify the data that the animation samples, set one of the `frames` properties that matches the animated property’s type. For example, set the frames property to interpolate Float values.

The following code designates a SampledAnimation to animate a propery of type Float by specifying the generic typed syntax. The code queues an array of values: `1.0`, `2.0`, and `3.0`.

```
// Define the animation type.
typealias SampledAnimationType = SampledAnimation

// Define the animated property values.
let frameArray: [Float] = [1.0, 2.0, 3.0]
```

To determine how fast the animation progresses from frame to frame, define this structure’s frameInterval property. The following code specifies a one-second delay between value changes before initializing the animation object.

```
// Define a one-second frame interval.
let interval: TimeInterval = 1

// Create the animation.
let sampleAnim = SampledAnimationType(
    frames: frameArray,
    name: "sampledAnim1",
    frameInterval: interval
    isAdditive: true,
    bindTarget: .transform,
    blendLayer: 100,
    repeatMode: .autoReverse,
    fillMode: .backwards,
    trimStart: 1.0,
    trimEnd: 10.0,
    trimDuration: 9.0,
    offset: 2.0,
    delay: 1.0,
    speed: 2.0
)
```

## Topics

### Creating an animation

init(frames: [Value], name: String, tweenMode: TweenMode, frameInterval: Float, isAdditive: Bool, bindTarget: BindTarget?, blendLayer: Int32, repeatMode: AnimationRepeatMode, fillMode: AnimationFillMode, trimStart: TimeInterval?, trimEnd: TimeInterval?, trimDuration: TimeInterval?, offset: TimeInterval, delay: TimeInterval, speed: Float)

Creates an animation with a collection of frames that represent incremental steps in the overall timeline.

init(jointNames: [String], frames: [Value], name: String, tweenMode: TweenMode, frameInterval: Float, isAdditive: Bool, isScaleAnimated: Bool, isRotationAnimated: Bool, isTranslationAnimated: Bool, bindTarget: BindTarget?, blendLayer: Int32, repeatMode: AnimationRepeatMode, fillMode: AnimationFillMode, trimStart: TimeInterval?, trimEnd: TimeInterval?, trimDuration: TimeInterval?, offset: TimeInterval, delay: TimeInterval, speed: Float)

Creates an animation that interpolates between two configurations of the given joints.

### Configuring the animation

var name: String

A textual name for the animation.

var bindTarget: BindTarget

A textual name that identifies the particular property that animates.

var blendLayer: Int32

The order in which the framework composites the animation.

var jointNames: [String]

The names of the joints to animate.

var isRotationAnimated: Bool

A Boolean value that indicates whether the animation observes rotational changes in the entity’s transform.

var isScaleAnimated: Bool

A Boolean value that indicates whether the animation observes changes in the entity’s size.

var isTranslationAnimated: Bool

A Boolean value that indicates whether the animation observes translational changes in the entity’s transform.

var additive: Bool

A Boolean value that indicates whether the animation builds on the current state of the target entity or resets the state before running.

var tweenMode: TweenMode

An option that determines how animation frames transition.

### Defining frames data

var frames: [JointTransforms]

An array of joint transforms in which each element represents a discrete state of the target entity at a given point in the animation’s timeline.

var frames: [Transform]

An array of transforms in which each element represents a discrete state of the target entity at a given point in the animation’s timeline.

var frames: [Double]

An array of double-precision values in which each element represents a discrete state of the animated property at a given point in the animation’s timeline.

var frames: [Float]

An array of floating-point values in which each element represents a discrete state of the animated property at a given point in the animation’s timeline.

var frames: [simd_quatf]

An array of quaternions in which each element represents a discrete state of the animated property at a given point in the animation’s timeline.

var frames: [SIMD2&lt;Float>]

An array of floating-point pairs in which each element represents a discrete state of the animated property at a given point in the animation’s timeline.

var frames: [SIMD3&lt;Float>]

An array of floating-point triplets in which each element represents a discrete state of the animated property at a given point in the animation’s timeline.

var frames: [SIMD4&lt;Float>]

An array of floating-point quadruples in which each element represents a discrete state of the animated property at a given point in the animation’s timeline.

### Timing the animation

var frameInterval: Float

The duration within the animation timeline for each frame in the frames array.

var start: TimeInterval

An integer multiple of the frame interval at which the animation plays.

var end: TimeInterval

An integer multiple of the frame interval at which the animation stops.

var speed: Float

A factor that changes the animation’s rate of playback.

var delay: TimeInterval

An amount of time that elapses before the animation plays.

var duration: TimeInterval

The total playback time of the animation.

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

### Initializers

init(weightNames: [String], frames: [Value], name: String, tweenMode: TweenMode, frameInterval: Float, isAdditive: Bool, bindTarget: BindTarget?, blendLayer: Int32, repeatMode: AnimationRepeatMode, fillMode: AnimationFillMode, trimStart: TimeInterval?, trimEnd: TimeInterval?, trimDuration: TimeInterval?, offset: TimeInterval, delay: TimeInterval, speed: Float)

Creates an animation that blends between a configuration of blend targets.

### Instance Properties

var frames: [BlendShapeWeights]

An array of weights in which each element represents a discrete state of the target entity at a given point in the animation’s timeline.

var weightNames: [String]

The names of the weights to animate.

### Default Implementations

AnimationDefinition Implementations

## Relationships

### Conforms To

- AnimationDefinition

## See Also

### Animation definitions

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

struct AnimationGroup

A collection of animations that play simultaneously.

struct AnimationHandoffType

The type of handoff the play animation method performs between a current animation and a new animation.

