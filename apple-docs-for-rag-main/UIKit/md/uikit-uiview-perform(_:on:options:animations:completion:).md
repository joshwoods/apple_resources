

- UIKit
- UIView
-  perform(\_:on:options:animations:completion:) 

Type Method

# perform(\_:on:options:animations:completion:)

Performs a specified system-provided animation on one or more views, along with optional parallel animations that you define.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class func perform(
    _ animation: UIView.SystemAnimation,
    on views: [UIView],
    options: UIView.AnimationOptions = [],
    animations parallelAnimations: (() -> Void)?,
    completion: ((Bool) -> Void)? = nil
)
```

## Parameters 

`animation`  

The system animation to perform; a constant from the UIView.SystemAnimation enum.

`views`  

The views to perform the animations on.

`options`  

A mask of options indicating how you want to perform the animations. For a list of valid constants, see UIView.AnimationOptions.

`parallelAnimations`  

Additional animations you specify to run alongside the system animation, with the same timing and duration that the system animation defines or inherits.

In your additional animations, do not modify properties of the view on which the system animation is being performed.

`completion`  

A block object to be executed when the animation sequence ends. The single Boolean argument indicates whether or not the animations finished before the completion handler was called. If the animation duration is `0`, this block is performed at the beginning of the next run-loop cycle. You can use a `nil` value for this parameter.

## See Also

### Animating views

static func animate(with: Animation, changes: () -> Void, completion: (() -> Void)?)

Animates changes to one or more views using the specified SwiftUI animation.

class func animate(springDuration: TimeInterval, bounce: CGFloat, initialSpringVelocity: CGFloat, delay: TimeInterval, options: UIView.AnimationOptions, animations: () -> Void, completion: ((Bool) -> Void)?)

Animates changes to one or more views using a spring animation with the specified duration, bounce, initial velocity, delay, options, and completion handler.

class func animate(withDuration: TimeInterval, delay: TimeInterval, options: UIView.AnimationOptions, animations: () -> Void, completion: ((Bool) -> Void)?)

Animate changes to one or more views using the specified duration, delay, options, and completion handler.

class func animate(withDuration: TimeInterval, animations: () -> Void, completion: ((Bool) -> Void)?)

Animate changes to one or more views using the specified duration and completion handler.

class func animate(withDuration: TimeInterval, animations: () -> Void)

Animate changes to one or more views using the specified duration.

class func transition(with: UIView, duration: TimeInterval, options: UIView.AnimationOptions, animations: (() -> Void)?, completion: ((Bool) -> Void)?)

Creates a transition animation for the specified container view.

class func transition(from: UIView, to: UIView, duration: TimeInterval, options: UIView.AnimationOptions, completion: ((Bool) -> Void)?)

Creates a transition animation between the specified views using the given parameters.

class func animateKeyframes(withDuration: TimeInterval, delay: TimeInterval, options: UIView.KeyframeAnimationOptions, animations: () -> Void, completion: ((Bool) -> Void)?)

Creates an animation block object that can be used to set up keyframe-based animations for the current view.

class func addKeyframe(withRelativeStartTime: Double, relativeDuration: Double, animations: () -> Void)

Specifies the timing and animation values for a single frame of a keyframe animation.

class func animate(withDuration: TimeInterval, delay: TimeInterval, usingSpringWithDamping: CGFloat, initialSpringVelocity: CGFloat, options: UIView.AnimationOptions, animations: () -> Void, completion: ((Bool) -> Void)?)

Performs a view animation using a timing curve corresponding to the motion of a physical spring.

class func performWithoutAnimation(() -> Void)

Disables a view transition animation.

class func modifyAnimations(withRepeatCount: CGFloat, autoreverses: Bool, animations: () -> Void)

Repeats the specified animations a specific number of times, optionally running the animation forward and backward.

