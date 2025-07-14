

- SwiftUI
-  Animation 

Structure

# Animation

The way a view changes over time to create a smooth visual transition from one state to another.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct Animation
```

## Mentioned in 

Unifying your app’s animations

## Overview

An `Animation` provides a visual transition of a view when a state value changes from one value to another. The characteristics of this transition vary according to the animation type. For instance, a linear animation provides a mechanical feel to the animation because its speed is consistent from start to finish. In contrast, an animation that uses easing, like easeOut, offers a more natural feel by varying the acceleration of the animation.

To apply an animation to a view, add the animation(_:value:) modifier, and specify both an animation type and the value to animate. For instance, the Circle view in the following code performs an easeIn animation each time the state variable `scale` changes:

```
```

 Video with custom controls. 

 Content description: A video that shows a circle enlarging then shrinking to its original size using an ease-in animation. 

Play 

When the value of `scale` changes, the modifier scaleEffect(_:anchor:) resizes Circle according to the new value. SwiftUI can animate the transition between sizes because Circle conforms to the Shape protocol. Shapes in SwiftUI conform to the Animatable protocol, which describes how to animate a property of a view.

In addition to adding an animation to a view, you can also configure the animation by applying animation modifiers to the animation type. For example, you can:

- Delay the start of the animation by using the delay(_:) modifier.

- Repeat the animation by using the repeatCount(_:autoreverses:) or repeatForever(autoreverses:) modifiers.

- Change the speed of the animation by using the speed(_:) modifier.

For example, the Circle view in the following code repeats the easeIn animation three times by using the repeatCount(_:autoreverses:) modifier:

```
```

 Video with custom controls. 

 Content description: A video that shows a circle that repeats the ease-in animation three times: enlarging, then shrinking, then enlarging again. The animation reverses causing the circle to shrink, then enlarge, then shrink to its original size. 

Play 

A view can also perform an animation when a binding value changes. To specify the animation type on a binding, call its animation(_:) method. For example, the view in the following code performs a linear animation, moving the box truck between the leading and trailing edges of the view. The truck moves each time a person clicks the Toggle control, which changes the value of the `$isTrailing` binding.

```
```

 Video with custom controls. 

 Content description: A video that shows a box truck that moves from the leading edge of a view to the trailing edge. The box truck then returns to the view's leading edge. 

Play 

## Topics

### Getting the default animation

static let `default`: Animation

A default animation instance.

### Getting linear animations

static var linear: Animation

An animation that moves at a constant speed.

static func linear(duration: TimeInterval) -> Animation

An animation that moves at a constant speed during a specified duration.

### Getting eased animations

static var easeIn: Animation

An animation that starts slowly and then increases speed towards the end of the movement.

static func easeIn(duration: TimeInterval) -> Animation

An animation with a specified duration that starts slowly and then increases speed towards the end of the movement.

static var easeOut: Animation

An animation that starts quickly and then slows towards the end of the movement.

static func easeOut(duration: TimeInterval) -> Animation

An animation with a specified duration that starts quickly and then slows towards the end of the movement.

static var easeInOut: Animation

An animation that combines the behaviors of in and out easing animations.

static func easeInOut(duration: TimeInterval) -> Animation

An animation with a specified duration that combines the behaviors of in and out easing animations.

### Getting built-in spring animations

static var bouncy: Animation

A spring animation with a predefined duration and higher amount of bounce.

static func bouncy(duration: TimeInterval, extraBounce: Double) -> Animation

A spring animation with a predefined duration and higher amount of bounce that can be tuned.

static var smooth: Animation

A smooth spring animation with a predefined duration and no bounce.

static func smooth(duration: TimeInterval, extraBounce: Double) -> Animation

A smooth spring animation with a predefined duration and no bounce that can be tuned.

static var snappy: Animation

A spring animation with a predefined duration and small amount of bounce that feels more snappy.

static func snappy(duration: TimeInterval, extraBounce: Double) -> Animation

A spring animation with a predefined duration and small amount of bounce that feels more snappy and can be tuned.

### Customizing spring animations

static var spring: Animation

A persistent spring animation. When mixed with other `spring()` or `interactiveSpring()` animations on the same property, each animation will be replaced by their successor, preserving velocity from one animation to the next. Optionally blends the response values between springs over a time period.

static func spring(Spring, blendDuration: TimeInterval) -> Animation

A persistent spring animation.

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

### Creating custom animations

init&lt;A>(A)

Create an `Animation` that contains the specified custom animation.

static func timingCurve(UnitCurve, duration: TimeInterval) -> Animation

Creates a new animation with speed controlled by the given curve.

static func timingCurve(Double, Double, Double, Double, duration: TimeInterval) -> Animation

An animation created from a cubic Bézier timing curve.

### Configuring an animation

func delay(TimeInterval) -> Animation

Delays the start of the animation by the specified number of seconds.

func repeatCount(Int, autoreverses: Bool) -> Animation

Repeats the animation for a specific number of times.

func repeatForever(autoreverses: Bool) -> Animation

Repeats the animation for the lifespan of the view containing the animation.

func speed(Double) -> Animation

Changes the duration of an animation by adjusting its speed.

### Instance Properties

var base: any CustomAnimation

### Instance Methods

func animate&lt;V>(value: V, time: TimeInterval, context: inout AnimationContext&lt;V>) -> V?

Calculates the current value of the animation.

func logicallyComplete(after: TimeInterval) -> Animation

Causes the animation to report logical completion after the specified duration, if it has not already logically completed.

func shouldMerge&lt;V>(previous: Animation, value: V, time: TimeInterval, context: inout AnimationContext&lt;V>) -> Bool

Returns a Boolean value that indicates whether the current animation should merge with a previous animation.

func velocity&lt;V>(value: V, time: TimeInterval, context: AnimationContext&lt;V>) -> V?

Calculates the current velocity of the animation.

### Type Methods

static func interactiveSpring(duration: TimeInterval, extraBounce: Double, blendDuration: TimeInterval) -> Animation

A convenience for a `spring` animation with a lower `response` value, intended for driving interactive animations.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Adding state-based animation to an action

func withAnimation&lt;Result>(Animation?, () throws -> Result) rethrows -> Result

Returns the result of recomputing the view’s body with the provided animation.

func withAnimation&lt;Result>(Animation?, completionCriteria: AnimationCompletionCriteria, () throws -> Result, completion: () -> Void) rethrows -> Result

Returns the result of recomputing the view’s body with the provided animation, and runs the completion when all animations are complete.

struct AnimationCompletionCriteria

The criteria that determines when an animation is considered finished.

