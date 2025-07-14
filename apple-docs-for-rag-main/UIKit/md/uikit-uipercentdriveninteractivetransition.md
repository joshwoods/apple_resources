

- UIKit
-  UIPercentDrivenInteractiveTransition 

Class

# UIPercentDrivenInteractiveTransition

An object that drives an interactive animation between one view controller and another.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIPercentDrivenInteractiveTransition
```

## Overview

A percent-driven interactive transition object relies on a transition animator delegate—a custom object that adopts the UIViewControllerAnimatedTransitioning protocol—to set up and perform the animations.

To use this concrete class, return an instance of it from your view controller delegate when asked for an interactive transition controller. As user events arrive that would affect the progress of a transition, call the update(_:), cancel(), and finish() methods to reflect the current progress. For example, you might call these methods from a gesture recognizer to reflect how much of the gesture is completed.

You can subclass UIPercentDrivenInteractiveTransition, but if you do so you must start each of your method overrides with a call to the `super` implementation of the method.

## Topics

### Accessing transition attributes

var timingCurve: (any UITimingCurveProvider)?

The timing curve to use when driving the animations.

var completionCurve: UIView.AnimationCurve

Indicates the animation completion curve for an interactive transition.

var duration: CGFloat

The overall duration (in seconds) of the transition animation.

var percentComplete: CGFloat

The amount of the transition (specified as a percentage of the overall duration) that’s complete.

var completionSpeed: CGFloat

The speed of the transition animation.

var wantsInteractiveStart: Bool

A Boolean value indicating whether the animations are interactive initially.

### Managing a transition

func update(CGFloat)

Updates the completion percentage of the transition.

func pause()

Pauses an interruptible transition animation.

func cancel()

Notifies the system that user interactions canceled the transition.

func finish()

Notifies the system that user interactions signaled the completion of the transition.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable
- UIViewControllerInteractiveTransitioning

## See Also

### Interactive transitions

protocol UIViewControllerInteractiveTransitioning

A set of methods that enable an object (such as a navigation controller) to drive a view controller transition.

protocol UIViewImplicitlyAnimating

An interface for modifying an animation while it’s running.

