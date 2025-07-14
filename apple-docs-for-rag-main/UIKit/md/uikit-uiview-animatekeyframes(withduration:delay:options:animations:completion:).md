

- UIKit
- UIView
-  animateKeyframes(withDuration:delay:options:animations:completion:) 

Type Method

# animateKeyframes(withDuration:delay:options:animations:completion:)

Creates an animation block object that can be used to set up keyframe-based animations for the current view.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class func animateKeyframes(
    withDuration duration: TimeInterval,
    delay: TimeInterval,
    options: UIView.KeyframeAnimationOptions = [],
    animations: @escaping () -> Void,
    completion: ((Bool) -> Void)? = nil
)
```

``` source
@MainActor
class func animateKeyframes(
    withDuration duration: TimeInterval,
    delay: TimeInterval,
    options: UIView.KeyframeAnimationOptions = [],
    animations: @escaping () -> Void
) async -> Bool
```

## Parameters 

`duration`  

The duration of the overall animation, measured in seconds. If you specify a negative value or `0`, changes are made immediately and without animations.

`delay`  

Specifies the time (in seconds) to wait before starting the animation.

`options`  

A mask of options indicating how you want to perform the animations. For a list of valid constants, see UIView.KeyframeAnimationOptions.

`animations`  

A block object containing the changes to commit to the views. Typically, you call the addKeyframe(withRelativeStartTime:relativeDuration:animations:) method one or more times from inside this block. You may also change view values directly if you want those changes to animate over the full duration. This block takes no parameters and has no return value. Do not use a `nil` value for this parameter.

`completion`  

A block object to be executed when the animation sequence ends. This block has no return value and takes a single Boolean argument that indicates whether or not the animations finished before the completion handler was called. If the duration of the animation is 0, this block is performed at the beginning of the next run loop cycle. You can use a `nil` value for this parameter.

## Discussion

This method creates an animation block that you can use to set up a keyframe-based animation. The keyframes themselves are not part of the initial animation block you create using this method. Inside the `animations` block, you must add the keyframe time and animation data by calling the addKeyframe(withRelativeStartTime:relativeDuration:animations:) method one or more times. Adding keyframes causes the animation to animate the view from its current value to the value of the first keyframe, then to the value of the next keyframe, and so on at the times you specify.

If you do not add any keyframes in the `animations` block, the animation proceeds from start to end like a standard animation block. In other words, the system animates from the current view values to any new values over the specified `duration`.

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

