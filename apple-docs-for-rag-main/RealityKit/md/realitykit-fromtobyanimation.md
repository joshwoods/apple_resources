

- RealityKit
-  FromToByAnimation 

Structure

# FromToByAnimation

An animation that starts, stops, or increments by a specific value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct FromToByAnimation where Value : AnimatableData
```

## Overview

To animate an entity or scene, this structure gradually changes a parameter’s value over time. You can specify a *from* value, which represents the animated property’s initial value at the beginning of the animation. You can also specify a *to* value, which determines the value of the property at the end of the animation. Alternatively, you can set a *by* value. The framework adds the *by* value to the property’s initial state to calculate the value at the end of the animation.

To specify the property that this struct animates, define `bindTarget` in the intializer,

init(name:from:to:by:duration:timing:isAdditive:bindTarget:blendLayer:repeatMode:fillMode:trimStart:trimEnd:trimDuration:offset:delay:speed:).

### Configure the animation inputs

This animation supports varying input combinations, which exhibit the following behavior. When you specify:

A *from* and *to* value  
The animation interpolates between *from* and *to*, and ignores the *by* value.

A *from* and *by* value  
The animation interpolates between *from* and the sum of *from* and *by*.

Only a *from* value  
The animation interpolates between *from* and the default source value.

Only a *to* value  
The animation interpolates between the default source value and *to*.

A *to* and *by* value  
The animation starts at *by* subtracted from \_to \_and completes at *to*.

Only a *by* value  
The animation interpolates between the default source value and the sum of default source value and *by*.

No *from*, *to*, or *by* value  
The animation interpolates between the default source value and the default target value.

The default source value is the base value of the of animated property. If multiple animations target the property, then the framework observes the output of the previous animation as the subsequent animation’s default source value. The default target value is the base value of the animated property.

## Topics

### Creating an animation

init(name: String, from: Value?, to: Value?, by: Value?, duration: TimeInterval, timing: AnimationTimingFunction, isAdditive: Bool, bindTarget: BindTarget?, blendLayer: Int32, repeatMode: AnimationRepeatMode, fillMode: AnimationFillMode, trimStart: TimeInterval?, trimEnd: TimeInterval?, trimDuration: TimeInterval?, offset: TimeInterval, delay: TimeInterval, speed: Float)

Creates an animation that interpolates between two values for a property of the target entity.

init(jointNames: [String], name: String, isScaleAnimated: Bool, isRotationAnimated: Bool, isTranslationAnimated: Bool, from: Value?, to: Value?, by: Value?, duration: TimeInterval, timing: AnimationTimingFunction, isAdditive: Bool, bindTarget: BindTarget?, blendLayer: Int32, repeatMode: AnimationRepeatMode, fillMode: AnimationFillMode, trimStart: TimeInterval?, trimEnd: TimeInterval?, trimDuration: TimeInterval?, offset: TimeInterval, delay: TimeInterval, speed: Float)

Creates an animation that interpolates between two configurations of the given joints.

### Configuring the animation

var name: String

A textual name for the animation.

var bindTarget: BindTarget

A textual name that identifies the particular property that animates.

var blendLayer: Int32

The order in which the framework composites the animation.

var jointNames: [String]

Joint names that define the joints in the skeletal pose.

var isScaleAnimated: Bool

A Boolean value that indicates whether that animation interpolates changes to the target’s size.

var isRotationAnimated: Bool

A Boolean value that indicates whether the animation interpolates rotational changes.

var isTranslationAnimated: Bool

A Boolean value that indicates whether the animation interpolates changes to the target object’s position.

var isAdditive: Bool

A Boolean value that indicates whether the animation blends additively with concurrent animations.

### Defining a start value

var fromValue: JointTransforms?

var fromValue: Transform?

var fromValue: Double?

var fromValue: Float?

var fromValue: simd_quatf?

var fromValue: SIMD2&lt;Float>?

var fromValue: SIMD3&lt;Float>?

var fromValue: SIMD4&lt;Float>?

### Defining an incremental value

var byValue: JointTransforms?

var byValue: Transform?

var byValue: Double?

var byValue: Float?

var byValue: simd_quatf?

var byValue: SIMD2&lt;Float>?

var byValue: SIMD3&lt;Float>?

var byValue: SIMD4&lt;Float>?

### Defining an end value

var toValue: JointTransforms?

var toValue: Transform?

var toValue: Double?

var toValue: Float?

var toValue: simd_quatf?

var toValue: SIMD2&lt;Float>?

var toValue: SIMD3&lt;Float>?

var toValue: SIMD4&lt;Float>?

### Timing the animation

var speed: Float

A factor that increases or decreases the animation’s rate of playback.

var delay: TimeInterval

An amount of time that elapses before the animation plays.

var duration: TimeInterval

The total playback time of the animation.

var offset: TimeInterval

The time, in seconds, at which the animation begins within the duration.

var timing: AnimationTimingFunction

An option that determines the animation’s pace over time.

var trimDuration: TimeInterval?

An optional duration that overrides the calculated duration.

var trimStart: TimeInterval?

The time, in seconds, at which the animation plays.

var trimEnd: TimeInterval?

The time, in seconds, at which the animation stops.

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

init(weightNames: [String], name: String, from: Value?, to: Value?, by: Value?, duration: TimeInterval, timing: AnimationTimingFunction, isAdditive: Bool, bindTarget: BindTarget?, blendLayer: Int32, repeatMode: AnimationRepeatMode, fillMode: AnimationFillMode, trimStart: TimeInterval?, trimEnd: TimeInterval?, trimDuration: TimeInterval?, offset: TimeInterval, delay: TimeInterval, speed: Float)

Creates an animation that blends between a configuration of blend targets.

### Instance Properties

var byValue: BlendShapeWeights?

var fromValue: BlendShapeWeights?

var toValue: BlendShapeWeights?

var weightNames: [String]

Weight names that define the weights for the blend shape.

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

