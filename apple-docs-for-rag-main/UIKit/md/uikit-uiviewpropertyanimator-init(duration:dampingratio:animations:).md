

- UIKit
- UIViewPropertyAnimator
-  init(duration:dampingRatio:animations:) 

Initializer

# init(duration:dampingRatio:animations:)

Initializes the animator object with spring-based timing information.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
convenience init(
    duration: TimeInterval,
    dampingRatio ratio: CGFloat,
    animations: (() -> Void)? = nil
)
```

## Parameters 

`duration`  

The duration of the animation, in seconds.

`ratio`  

The damping ratio to apply to the initial acceleration and oscillation. To smoothly decelerate the animation without oscillation, specify a value of `1`. Specify values closer to `0` to create less damping and more oscillation.

`animations`  

The block containing the animations. This block has no return value and takes no parameters. Use this block to modify any animatable view properties. When you start the animations, those properties are animated from their current values to the new values using the specified animation parameters.

## Return Value

An initialized animator object or `nil` if the object could not be created.

## Discussion

Spring-based animations cause the value of a property to accelerate initially toward its new value and then oscillate around that value until before finally coming to rest on the value. The initial amount of acceleration is proportional to the difference between the start and end values of the property. In other words, the greater the difference between the start and end values, the greater the initial acceleration. The `ratio` parameter determines the amount of damping applied to the initial acceleration. Lower damping values correspond to less resistance to the acceleration and more oscillation before coming to rest. Higher damping values correspond to more resistance and less oscillation.

The animator object returned by this method begins in the UIViewAnimatingState.inactive state. You must explicitly start the animations by calling the startAnimation() method.

## See Also

### Initializing a property animator

convenience init(duration: TimeInterval, curve: UIView.AnimationCurve, animations: (() -> Void)?)

Initializes the animator with a built-in UIKit timing curve.

convenience init(duration: TimeInterval, controlPoint1: CGPoint, controlPoint2: CGPoint, animations: (() -> Void)?)

Initializes the animator object with a cubic Bézier timing curve.

init(duration: TimeInterval, timingParameters: any UITimingCurveProvider)

Initializes the animator object with a custom timing curve object.

class func runningPropertyAnimator(withDuration: TimeInterval, delay: TimeInterval, options: UIView.AnimationOptions, animations: () -> Void, completion: ((UIViewAnimatingPosition) -> Void)?) -> Self

Creates and returns an animator object that begins running its animations immediately.

