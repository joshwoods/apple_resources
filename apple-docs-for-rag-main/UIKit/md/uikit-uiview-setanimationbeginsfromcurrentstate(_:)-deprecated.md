

- UIKit
- UIView
-  setAnimationBeginsFromCurrentState(\_:) Deprecated

Type Method

# setAnimationBeginsFromCurrentState(\_:)

Sets whether the animation should begin playing from the current state.

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
class func setAnimationBeginsFromCurrentState(_ fromCurrentState: Bool)
```

## Parameters 

`fromCurrentState`  

Specify true if animations should begin from their currently visible state; otherwise, false.

## Discussion

If set to true when an animation is in flight, the current view position of the in-flight animation is used as the starting state for the new animation. If set to false, the in-flight animation ends before the new animation begins using the last view position as the starting state. This method does nothing if an animation is not in flight or invoked outside of an animation block. Use the beginAnimations(_:context:) class method to start and the commitAnimations() class method to end an animation block. The default value is false.

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

class func setAnimationRepeatAutoreverses(Bool)

Sets whether the animations within an animation block automatically reverse themselves.

Deprecated

class func setAnimationTransition(UIView.AnimationTransition, for: UIView, cache: Bool)

Sets a transition to apply to a view during an animation block.

Deprecated

class var areAnimationsEnabled: Bool

Returns a Boolean value indicating whether animations are enabled.

func forBaselineLayout() -> UIView

Returns a view used to satisfy baseline constraints.

Deprecated

