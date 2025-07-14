

- UIKit
- UIViewPropertyAnimator
-  runningPropertyAnimator(withDuration:delay:options:animations:completion:) 

Type Method

# runningPropertyAnimator(withDuration:delay:options:animations:completion:)

Creates and returns an animator object that begins running its animations immediately.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
class func runningPropertyAnimator(
    withDuration duration: TimeInterval,
    delay: TimeInterval,
    options: UIView.AnimationOptions = [],
    animations: @escaping () -> Void,
    completion: ((UIViewAnimatingPosition) -> Void)? = nil
) -> Self
```

## Parameters 

`duration`  

The duration of the animation, in seconds.

`delay`  

The number of seconds to wait before starting the animations. Specify 0 to begin the animations immediately.

`options`  

The options to apply to the animations. You can specify most options, but transition-related options and options related to the animation direction are ignored. For a list of options, see UIView.AnimationOptions.

`animations`  

The block containing the animations. This block has no return value and takes no parameters. Use this block to modify any animatable properties of your view. Those properties are animated from their current values to the new values using the specified animation parameters.

`completion`  

The block to execute when the animations finish. You can use this block to perform any final actions. This block has no return value and takes the following parameter:

finalPosition  
The ending position of the animations. Use this value to determine whether the animations stopped at the beginning, end, or somewhere in the middle.

## Return Value

An initialized animator object or `nil` if the object could not be created.

## Discussion

This method creates the property animator object, configures it, and calls its startAnimation() method after the specified delay. If you don’t specify an animation curve in the options parameter, this method uses the curveEaseInOut option.

## See Also

### Initializing a property animator

convenience init(duration: TimeInterval, curve: UIView.AnimationCurve, animations: (() -> Void)?)

Initializes the animator with a built-in UIKit timing curve.

convenience init(duration: TimeInterval, controlPoint1: CGPoint, controlPoint2: CGPoint, animations: (() -> Void)?)

Initializes the animator object with a cubic Bézier timing curve.

convenience init(duration: TimeInterval, dampingRatio: CGFloat, animations: (() -> Void)?)

Initializes the animator object with spring-based timing information.

init(duration: TimeInterval, timingParameters: any UITimingCurveProvider)

Initializes the animator object with a custom timing curve object.

