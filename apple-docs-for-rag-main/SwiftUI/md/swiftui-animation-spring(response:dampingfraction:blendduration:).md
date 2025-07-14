

- SwiftUI
- Animation
-  spring(response:dampingFraction:blendDuration:) 

Type Method

# spring(response:dampingFraction:blendDuration:)

A persistent spring animation. When mixed with other `spring()` or `interactiveSpring()` animations on the same property, each animation will be replaced by their successor, preserving velocity from one animation to the next. Optionally blends the response values between springs over a time period.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func spring(
    response: Double = 0.5,
    dampingFraction: Double = 0.825,
    blendDuration: TimeInterval = 0
) -> Animation
```

## Parameters 

`response`  

The stiffness of the spring, defined as an approximate duration in seconds. A value of zero requests an infinitely-stiff spring, suitable for driving interactive animations.

`dampingFraction`  

The amount of drag applied to the value being animated, as a fraction of an estimate of amount needed to produce critical damping.

`blendDuration`  

The duration in seconds over which to interpolate changes to the response value of the spring.

## Return Value

A spring animation.

## See Also

### Customizing spring animations

static var spring: Animation

A persistent spring animation. When mixed with other `spring()` or `interactiveSpring()` animations on the same property, each animation will be replaced by their successor, preserving velocity from one animation to the next. Optionally blends the response values between springs over a time period.

static func spring(Spring, blendDuration: TimeInterval) -> Animation

A persistent spring animation.

static func spring(duration: TimeInterval, bounce: Double, blendDuration: Double) -> Animation

A persistent spring animation. When mixed with other `spring()` or `interactiveSpring()` animations on the same property, each animation will be replaced by their successor, preserving velocity from one animation to the next. Optionally blends the duration values between springs over a time period.

static var interactiveSpring: Animation

A convenience for a `spring` animation with a lower `duration` value, intended for driving interactive animations.

static func interactiveSpring(response: Double, dampingFraction: Double, blendDuration: TimeInterval) -> Animation

A convenience for a `spring` animation with a lower `response` value, intended for driving interactive animations.

static var interpolatingSpring: Animation

An interpolating spring animation that uses a damped spring model to produce values in the range \[0, 1\] that are then used to interpolate within the \[from, to\] range of the animated property. Preserves velocity across overlapping animations by adding the effects of each animation.

static func interpolatingSpring(Spring, initialVelocity: Double) -> Animation

An interpolating spring animation that uses a damped spring model to produce values in the range of one to zero.

static func interpolatingSpring(duration: TimeInterval, bounce: Double, initialVelocity: Double) -> Animation

An interpolating spring animation that uses a damped spring model to produce values in the range \[0, 1\] that are then used to interpolate within the \[from, to\] range of the animated property. Preserves velocity across overlapping animations by adding the effects of each animation.

static func interpolatingSpring(mass: Double, stiffness: Double, damping: Double, initialVelocity: Double) -> Animation

An interpolating spring animation that uses a damped spring model to produce values in the range \[0, 1\] that are then used to interpolate within the \[from, to\] range of the animated property. Preserves velocity across overlapping animations by adding the effects of each animation.

