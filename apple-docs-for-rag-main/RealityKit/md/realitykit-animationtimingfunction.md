

- RealityKit
-  AnimationTimingFunction 

Structure

# AnimationTimingFunction

The pacing of an animation transition.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
struct AnimationTimingFunction
```

## Overview

Use an animation timing function to control the pace of an animation transition when you call one of an entity’s animated move methods, like move(to:relativeTo:duration:timingFunction:). If you omit a timing function from the call, the method uses the default timing function.

## Topics

### Creating timing functions

static var `default`: AnimationTimingFunction

A timing function that produces the default curve for the transition.

static var easeIn: AnimationTimingFunction

A timing function that produces a gradual starting transition.

static var easeInOut: AnimationTimingFunction

A timing function that produces a gradual starting and ending transition.

static var easeOut: AnimationTimingFunction

A timing function that produces a gradual ending transition.

static var linear: AnimationTimingFunction

A timing function that produces a linear transition.

static func cubicBezier(controlPoint1: SIMD2&lt;Float>, controlPoint2: SIMD2&lt;Float>) -> AnimationTimingFunction

Creates a timing function that accelerates and then decelerates towards the target value with the cubic bezier shape specified by two control points.

### Comparing timing functions

static func == (AnimationTimingFunction, AnimationTimingFunction) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

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
- Hashable

## See Also

### Animation definitions

struct SampledAnimation

An animation that cycles through a series of frames at a constant interval.

enum TweenMode

Options that determine whether an animation switches between frames gradually or abruptly.

struct FromToByAnimation

An animation that starts, stops, or increments by a specific value.

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

