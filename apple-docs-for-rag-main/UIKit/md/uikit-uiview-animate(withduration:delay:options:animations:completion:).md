

- UIKit
- UIView
-  animate(withDuration:delay:options:animations:completion:) 

Type Method

# animate(withDuration:delay:options:animations:completion:)

Animate changes to one or more views using the specified duration, delay, options, and completion handler.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class func animate(
    withDuration duration: TimeInterval,
    delay: TimeInterval,
    options: UIView.AnimationOptions = [],
    animations: @escaping () -> Void,
    completion: ((Bool) -> Void)? = nil
)
```

## Parameters 

`duration`  

The total duration of the animations, measured in seconds. If you specify a negative value or `0`, the changes are made without animating them.

`delay`  

The amount of time (measured in seconds) to wait before beginning the animations. Specify a value of `0` to begin the animations immediately.

`options`  

A mask of options indicating how you want to perform the animations. For a list of valid constants, see UIView.AnimationOptions.

`animations`  

A block object containing the changes to commit to the views. This is where you programmatically change any animatable properties of the views in your view hierarchy. This block takes no parameters and has no return value. This parameter must not be `NULL`.

`completion`  

A block object to be executed when the animation sequence ends. This block has no return value and takes a single Boolean argument that indicates whether or not the animations actually finished before the completion handler was called. If the duration of the animation is 0, this block is performed at the beginning of the next run loop cycle. This parameter may be `NULL`.

## Discussion

This method initiates a set of animations to perform on the view. The block object in the `animations` parameter contains the code for animating the properties of one or more views.

During an animation, user interactions are temporarily disabled for the views being animated. (Prior to iOS 5, user interactions are disabled for the entire application.) If you want users to be able to interact with the views, include the allowUserInteraction constant in the `options` parameter.

## See Also

### Animating views

static func animate(with: Animation, changes: () -> Void, completion: (() -> Void)?)

Animates changes to one or more views using the specified SwiftUI animation.

class func animate(springDuration: TimeInterval, bounce: CGFloat, initialSpringVelocity: CGFloat, delay: TimeInterval, options: UIView.AnimationOptions, animations: () -> Void, completion: ((Bool) -> Void)?)

Animates changes to one or more views using a spring animation with the specified duration, bounce, initial velocity, delay, options, and completion handler.

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

class func perform(UIView.SystemAnimation, on: [UIView], options: UIView.AnimationOptions, animations: (() -> Void)?, completion: ((Bool) -> Void)?)

Performs a specified system-provided animation on one or more views, along with optional parallel animations that you define.

class func animate(withDuration: TimeInterval, delay: TimeInterval, usingSpringWithDamping: CGFloat, initialSpringVelocity: CGFloat, options: UIView.AnimationOptions, animations: () -> Void, completion: ((Bool) -> Void)?)

Performs a view animation using a timing curve corresponding to the motion of a physical spring.

class func performWithoutAnimation(() -> Void)

Disables a view transition animation.

class func modifyAnimations(withRepeatCount: CGFloat, autoreverses: Bool, animations: () -> Void)

Repeats the specified animations a specific number of times, optionally running the animation forward and backward.

