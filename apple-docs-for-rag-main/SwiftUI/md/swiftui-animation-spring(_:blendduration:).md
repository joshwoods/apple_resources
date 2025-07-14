

- SwiftUI
- Animation
-  spring(\_:blendDuration:) 

Type Method

# spring(\_:blendDuration:)

A persistent spring animation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func spring(
    _ spring: Spring,
    blendDuration: TimeInterval = 0.0
) -> Animation
```

## Discussion

When mixed with other `spring()` or `interactiveSpring()` animations on the same property, each animation will be replaced by their successor, preserving velocity from one animation to the next. Optionally blends the duration values between springs over a time period.

## See Also

### Customizing spring animations

static var spring: Animation

A persistent spring animation. When mixed with other `spring()` or `interactiveSpring()` animations on the same property, each animation will be replaced by their successor, preserving velocity from one animation to the next. Optionally blends the response values between springs over a time period.

static func spring(duration: TimeInterval, bounce: Double, blendDuration: Double) -> Animation

A persistent spring animation. When mixed with other `spring()` or `interactiveSpring()` animations on the same property, each animation will be replaced by their successor, preserving velocity from one animation to the next. Optionally blends the duration values between springs over a time period.

static func spring(response: Double, dampingFraction: Double, blendDuration: TimeInterval) -> Animation

A persistent spring animation. When mixed with other `spring()` or `interactiveSpring()` animations on the same property, each animation will be replaced by their successor, preserving velocity from one animation to the next. Optionally blends the response values between springs over a time period.

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

