

- UIKit
- UIView
-  setAnimationRepeatCount(\_:) Deprecated

Type Method

# setAnimationRepeatCount(\_:)

Sets the number of times animations within an animation block repeat.

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
class func setAnimationRepeatCount(_ repeatCount: Float)
```

## Parameters 

`repeatCount`  

The number of times animations repeat. This value can be a fraction. If you specify the value `0`, the animation is performed once without repeating.

## Discussion

Use this method to specify the number of times to repeat the specified animations. This method does nothing if called from outside of an animation block. You can use this method in conjunction with either the block-based methods or the begin/commit methods for defining an animation block. If you do not explicitly set a repeat count, the animation is not repeated.

If you pass the repeat option to the animate(withDuration:delay:options:animations:completion:) method without setting an explicit repeat count, the animation repeats indefinitely. If you want the animation to repeat a finite number of times, call this method from inside your block.

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

class func setAnimationRepeatAutoreverses(Bool)

Sets whether the animations within an animation block automatically reverse themselves.

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

