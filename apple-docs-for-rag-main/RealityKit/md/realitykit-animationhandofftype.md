

- RealityKit
-  AnimationHandoffType 

Structure

# AnimationHandoffType

The type of handoff the play animation method performs between a current animation and a new animation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct AnimationHandoffType
```

## Topics

### Operators

static func == (AnimationHandoffType, AnimationHandoffType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Type Properties

static var compose: AnimationHandoffType

Adds the new animation to existing animations, and immediately starts the new animation.

static var `default`: AnimationHandoffType

Provides the default behavior.

static var stop: AnimationHandoffType

Stops the specified animation.

### Type Methods

static func replace(applyToAllLayers: Bool) -> AnimationHandoffType

Keeps playing the current animation during the transition time and uses the value from that animation as the blend value for the transition to the new animation.

static func snapshotAndReplace(applyToAllLayers: Bool) -> AnimationHandoffType

Stops the current animation and uses the current value of that animation as the blend value for the transition to the new animation.

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable

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

struct AnimationGroup

A collection of animations that play simultaneously.

