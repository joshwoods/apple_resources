

- SwiftUI
-  Spring 

Structure

# Spring

A representation of a spring’s motion.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct Spring
```

## Overview

Use this type to convert between different representations of spring parameters:

```
let spring = Spring(duration: 0.5, bounce: 0.3)
let (mass, stiffness, damping) = (spring.mass, spring.stiffness, spring.damping)
// (1.0, 157.9, 17.6)

let spring2 = Spring(mass: 1, stiffness: 100, damping: 10)
let (duration, bounce) = (spring2.duration, spring2.bounce)
// (0.63, 0.5)
```

You can also use it to query for a spring’s position and its other properties for a given set of inputs:

```
func unitPosition(time: TimeInterval) -> Double {
    let spring = Spring(duration: 0.5, bounce: 0.3)
    return spring.position(target: 1.0, time: time)
}
```

## Topics

### Creating a spring

init(duration: TimeInterval, bounce: Double)

Creates a spring with the specified duration and bounce.

init(mass: Double, stiffness: Double, damping: Double, allowOverDamping: Bool)

Creates a spring with the specified mass, stiffness, and damping.

init(response: Double, dampingRatio: Double)

Creates a spring with the specified response and damping ratio.

init(settlingDuration: TimeInterval, dampingRatio: Double, epsilon: Double)

Creates a spring with the specified duration and damping ratio.

### Getting built-in springs

static var bouncy: Spring

A spring with a predefined duration and higher amount of bounce.

static func bouncy(duration: TimeInterval, extraBounce: Double) -> Spring

A spring with a predefined duration and higher amount of bounce that can be tuned.

static var smooth: Spring

A smooth spring with a predefined duration and no bounce.

static func smooth(duration: TimeInterval, extraBounce: Double) -> Spring

A smooth spring with a predefined duration and no bounce that can be tuned.

static var snappy: Spring

A spring with a predefined duration and small amount of bounce that feels more snappy.

static func snappy(duration: TimeInterval, extraBounce: Double) -> Spring

A spring with a predefined duration and small amount of bounce that feels more snappy and can be tuned.

### Getting spring characteristics

var bounce: Double

How bouncy the spring is.

var damping: Double

Defines how the spring’s motion should be damped due to the forces of friction.

var dampingRatio: Double

The amount of drag applied, as a fraction of the amount needed to produce critical damping.

var duration: TimeInterval

The perceptual duration, which defines the pace of the spring.

var mass: Double

The mass of the object attached to the end of the spring.

var response: Double

The stiffness of the spring, defined as an approximate duration in seconds.

var settlingDuration: TimeInterval

The estimated duration required for the spring system to be considered at rest.

var stiffness: Double

The spring stiffness coefficient.

### Getting spring state

func value&lt;V>(target: V, initialVelocity: V, time: TimeInterval) -> V

Calculates the value of the spring at a given time given a target amount of change.

func value&lt;V>(fromValue: V, toValue: V, initialVelocity: V, time: TimeInterval) -> V

Calculates the value of the spring at a given time for a starting and ending value for the spring to travel.

func velocity&lt;V>(target: V, initialVelocity: V, time: TimeInterval) -> V

Calculates the velocity of the spring at a given time given a target amount of change.

func velocity&lt;V>(fromValue: V, toValue: V, initialVelocity: V, time: TimeInterval) -> V

Calculates the velocity of the spring at a given time given a starting and ending value for the spring to travel.

### Setting spring state

func update&lt;V>(value: inout V, velocity: inout V, target: V, deltaTime: TimeInterval)

Updates the current value and velocity of a spring.

### Calculating forces and durations

func force&lt;V>(target: V, position: V, velocity: V) -> V

Calculates the force upon the spring given a current position, target, and velocity amount of change.

func force&lt;V>(fromValue: V, toValue: V, position: V, velocity: V) -> V

Calculates the force upon the spring given a current position, velocity, and divisor from the starting and end values for the spring to travel.

func settlingDuration&lt;V>(target: V, initialVelocity: V, epsilon: Double) -> TimeInterval

The estimated duration required for the spring system to be considered at rest.

func settlingDuration&lt;V>(fromValue: V, toValue: V, initialVelocity: V, epsilon: Double) -> TimeInterval

The estimated duration required for the spring system to be considered at rest.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Creating custom animations

protocol CustomAnimation

A type that defines how an animatable value changes over time.

struct AnimationContext

Contextual values that a custom animation can use to manage state and access a view’s environment.

struct AnimationState

A container that stores the state for a custom animation.

protocol AnimationStateKey

A key for accessing animation state values.

struct UnitCurve

A function defined by a two-dimensional curve that maps an input progress in the range \[0,1\] to an output progress that is also in the range \[0,1\]. By changing the shape of the curve, the effective speed of an animation or other interpolation can be changed.

