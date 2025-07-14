

- UIKit
-  UIViewPropertyAnimator 

Class

# UIViewPropertyAnimator

A class that animates changes to views and allows the dynamic modification of those animations.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
class UIViewPropertyAnimator
```

## Overview

A UIViewPropertyAnimator object lets you animate changes to views and dynamically modify your animations before they finish. With a property animator, you can run your animations from start to finish normally or you can turn them into interactive animations and control the timing yourself. The animator operates on animatable properties of views, such as the frame, center, alpha, and transform properties, creating the needed animations from the blocks you provide.

When creating a property animator object, you specify the following:

- A block containing code that modifies the properties of one or more views.

- The timing curve that defines the speed of the animation over the course of its run.

- The duration (in seconds) of the animation.

- An optional completion block to execute when the animations finish.

In your animation blocks, set the value of an animatable property to the final value you want reflected by that view. For example, if you want to fade out a view, you would set its alpha property to `0` in your block. The property animator object creates an animation that adjusts the value of that property from its initial value to the new value that you specified in your block.

The speed at which the value of a property changes is controlled by the timing curve you specify when creating the property animator. Property animators include support for the built-in UIKit animation curves such as linear, ease-in, and ease-out. You can also use a cubic Bezier curve or a spring function to control the timing of the animations.

If you create your animator using one of the standard initialization methods, you must explicitly start your animations by calling the startAnimation() method. If you want to start the animations immediately after the creation of your animator, use the runningPropertyAnimator(withDuration:delay:options:animations:completion:) method instead of the standard initializers.

This class adopts the UIViewAnimating and UIViewImplicitlyAnimating protocols, which define the methods for starting, stopping, and modifying your animations. For more information about the methods of those protocols, see UIViewAnimating and UIViewImplicitlyAnimating.

### Modify animations dynamically

A property animator gives you programmatic control over the timing and execution of the animations. Specifically, you can:

- Start, pause, resume, and stop animations; see the methods of the UIViewAnimating protocol.

- Add animation blocks after the original animations start using the addAnimations(_:) and addAnimations(_:delayFactor:) methods.

- Scrub through a paused animation by modifying the fractionComplete property.

- Change the animation’s direction using the isReversed property.

- Modify the timing and duration of a partially complete animation by pausing the animation and using the continueAnimation(withTimingParameters:durationFactor:) method to finish it.

Most of the basic behavior is controlled by the properties of the UIViewAnimating protocol, which this class adopts. Use those methods and properties to start, pause, resume, and stop the animations. You can also use them to scrub through the animation and change its direction. Use the methods and properties of this class to modify the animation blocks themselves and to update the timing information.

## Topics

### Initializing a property animator

convenience init(duration: TimeInterval, curve: UIView.AnimationCurve, animations: (() -> Void)?)

Initializes the animator with a built-in UIKit timing curve.

convenience init(duration: TimeInterval, controlPoint1: CGPoint, controlPoint2: CGPoint, animations: (() -> Void)?)

Initializes the animator object with a cubic Bézier timing curve.

convenience init(duration: TimeInterval, dampingRatio: CGFloat, animations: (() -> Void)?)

Initializes the animator object with spring-based timing information.

init(duration: TimeInterval, timingParameters: any UITimingCurveProvider)

Initializes the animator object with a custom timing curve object.

class func runningPropertyAnimator(withDuration: TimeInterval, delay: TimeInterval, options: UIView.AnimationOptions, animations: () -> Void, completion: ((UIViewAnimatingPosition) -> Void)?) -> Self

Creates and returns an animator object that begins running its animations immediately.

### Modifying animations

func addAnimations(() -> Void)

Adds the specified animation block to the animator.

func addAnimations(() -> Void, delayFactor: CGFloat)

Adds the specified animation block with a delay.

func addCompletion((UIViewAnimatingPosition) -> Void)

Adds the specified completion block to the animator.

func continueAnimation(withTimingParameters: (any UITimingCurveProvider)?, durationFactor: CGFloat)

Adjusts the timing and duration of a paused animation.

### Accessing the animation parameters

var duration: TimeInterval

The total duration (in seconds) of the main animations.

var delay: TimeInterval

The delay (in seconds) after which the animations begin.

var timingParameters: (any UITimingCurveProvider)?

The information used to determine the timing curve for the animation.

var isInterruptible: Bool

A Boolean value indicating whether the animator is interruptible and can be paused or stopped.

var isUserInteractionEnabled: Bool

A Boolean value indicating whether views receive touch events while animations are running.

var isManualHitTestingEnabled: Bool

A Boolean value indicating whether your app manages hit-testing while animations are in progress.

var scrubsLinearly: Bool

A Boolean value indicating whether a paused animation scrubs linearly or uses its specified timing information.

var pausesOnCompletion: Bool

A Boolean value that indicates whether a completed animation remains in the active state.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable
- UIViewAnimating
- UIViewImplicitlyAnimating

## See Also

### Essentials

protocol UIViewAnimating

An interface for implementing custom animator objects.

