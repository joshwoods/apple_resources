

- RealityKit
-  TweenMode 

Enumeration

# TweenMode

Options that determine whether an animation switches between frames gradually or abruptly.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
enum TweenMode
```

## Overview

This enumeration declares the options for a sampled animation’s tweenMode. The gradual or abrupt change, or *interpolation*, refers to the visual behavior that occurs between adjacent values in a sampled animation’s frames.

## Topics

### Choosing a mode between frames

case hold

An option that indicates a keyframe changes to the next abruptly.

case linear

An option that indicates that a keyframe changes to the next gradually.

### Comparing tween modes

static func == (TweenMode, TweenMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Animation definitions

struct SampledAnimation

An animation that cycles through a series of frames at a constant interval.

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

