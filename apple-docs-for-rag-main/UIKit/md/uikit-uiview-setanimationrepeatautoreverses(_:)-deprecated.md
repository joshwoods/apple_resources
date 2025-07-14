

- UIKit
- UIView
-  setAnimationRepeatAutoreverses(\_:) Deprecated

Type Method

# setAnimationRepeatAutoreverses(\_:)

Sets whether the animations within an animation block automatically reverse themselves.

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
class func setAnimationRepeatAutoreverses(_ repeatAutoreverses: Bool)
```

## Parameters 

`repeatAutoreverses`  

Specify true to enable autoreversing or false to disable it.

## Discussion

If you enable autoreversing, a single animation cycle changes the properties being animated to their new values and then back to their original values. At the end of the animations, the affected views are then updated immediately to reflect the new values. This method does nothing if called from outside of an animation block. By default, autoreversing is disabled.

If you combine autoreversing with a repeat count (settable using the setAnimationRepeatCount(_:) method), you can create animations that shift back and forth between the old and new values the specified number of times. However, remember that the repeat count indicates the number of complete cycles. If you specify an integral value such as `2.0`, the animation ends on the old value, which is followed by the view immediately updating itself to show the new value, which might be jarring. If you want the animation to end on the new value (instead of the old value), add `0.5` to the repeat count value. This adds an extra half cycle to the animation.

Use of this method is discouraged in iOS 4.0 and later. Instead, you should use theanimate(withDuration:delay:options:animations:completion:) method to specify your animations and the animation options.

## See Also

### Deprecated methods

class func beginAnimations(String?, context: UnsafeMutableRawPointer?)

Marks the beginning of a begin/commit animation block.

Deprecated

class func commitAnimations()

Marks the end of a begin/commit animation block and schedules the animations for execution.

Deprecated

class func setAnimationStart(Date)

Sets the start time for the current animation block.

Deprecated

class func setAnimationsEnabled(Bool)

Sets whether animations are enabled.

class func setAnimationDelegate(Any?)

Sets the delegate for any animation messages.

Deprecated

class func setAnimationWillStart(Selector?)

Sets the message to send to the animation delegate when the animation starts.

Deprecated

class func setAnimationDidStop(Selector?)

Sets the message to send to the animation delegate when animation stops.

Deprecated

class func setAnimationDuration(TimeInterval)

Sets the duration (measured in seconds) of the animations in an animation block.

Deprecated

class func setAnimationDelay(TimeInterval)

Sets the amount of time (in seconds) to wait before animating property changes within an animation block.

Deprecated

class func setAnimationCurve(UIView.AnimationCurve)

Sets the curve to use when animating property changes within an animation block.

Deprecated

class func setAnimationRepeatCount(Float)

Sets the number of times animations within an animation block repeat.

Deprecated

class func setAnimationBeginsFromCurrentState(Bool)

Sets whether the animation should begin playing from the current state.

Deprecated

class func setAnimationTransition(UIView.AnimationTransition, for: UIView, cache: Bool)

Sets a transition to apply to a view during an animation block.

Deprecated

class var areAnimationsEnabled: Bool

Returns a Boolean value indicating whether animations are enabled.

func forBaselineLayout() -> UIView

Returns a view used to satisfy baseline constraints.

Deprecated

