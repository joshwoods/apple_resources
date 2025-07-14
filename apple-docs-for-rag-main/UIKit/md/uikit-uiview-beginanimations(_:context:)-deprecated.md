

- UIKit
- UIView
-  beginAnimations(\_:context:) Deprecated

Type Method

# beginAnimations(\_:context:)

Marks the beginning of a begin/commit animation block.

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
class func beginAnimations(
    _ animationID: String?,
    context: UnsafeMutableRawPointer?
)
```

## Parameters 

`animationID`  

An application-supplied identifier for the animations.

`context`  

Custom data that you want to associate with this set of animations. information that is passed to the animation delegate messages—the selectors set using the setAnimationWillStart(_:) and setAnimationDidStop(_:) methods.

## Discussion

This method signals to the system that you want to specify one or more animations to perform. After calling this method, configure the animation options (using the `setAnimation…` class methods) and then change the desired animatable properties of your views. When you are done changing your view properties, call the commitAnimations() method to close the set and schedule the animations.

You can nest sets of animations (by calling this method again before committing a previous set of animations) as needed. Nesting animations groups them together and allows you to set different animation options for the nested group.

If you install a start or stop selector using the setAnimationWillStart(_:) or setAnimationDidStop(_:) method, the values you specify for the `animationID` and `context` parameters are passed to your selectors at runtime. You can use these parameters to pass additional information to those selectors.

Use of this method is discouraged in iOS 4.0 and later. You should use the block-based animation methods to specify your animations instead.

## See Also

### Deprecated methods

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

