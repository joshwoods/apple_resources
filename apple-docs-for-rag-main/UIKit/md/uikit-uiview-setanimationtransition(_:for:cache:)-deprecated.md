

- UIKit
- UIView
-  setAnimationTransition(\_:for:cache:) Deprecated

Type Method

# setAnimationTransition(\_:for:cache:)

Sets a transition to apply to a view during an animation block.

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
class func setAnimationTransition(
    _ transition: UIView.AnimationTransition,
    for view: UIView,
    cache: Bool
)
```

## Parameters 

`transition`  

A transition to apply to `view`. Possible values are described in UIView.AnimationTransition.

`view`  

The view to apply the transition to.

`cache`  

If true, the before and after images of `view` are rendered once and used to create the frames in the animation. Caching can improve performance but if you set this parameter to true, you must not update the view or its subviews during the transition. Updating the view and its subviews may interfere with the caching behaviors and cause the view contents to be rendered incorrectly (or in the wrong location) during the animation. You must wait until the transition ends to update the view.

If false, the view and its contents must be updated for each frame of the transition animation, which may noticeably affect the frame rate.

## Discussion

If you want to change the appearance of a view during a transition—for example, flip from one view to another—then use a container view, an instance of UIView, as follows:

1.  Begin an animation block.

2.  Set the transition on the container view.

3.  Remove the subview from the container view.

4.  Add the new subview to the container view.

5.  Commit the animation block.

Use of this method is discouraged in iOS 4.0 and later. You should use the transition(with:duration:options:animations:completion:) method to perform transitions instead.

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

class func setAnimationBeginsFromCurrentState(Bool)

Sets whether the animation should begin playing from the current state.

Deprecated

class var areAnimationsEnabled: Bool

Returns a Boolean value indicating whether animations are enabled.

func forBaselineLayout() -> UIView

Returns a view used to satisfy baseline constraints.

Deprecated

