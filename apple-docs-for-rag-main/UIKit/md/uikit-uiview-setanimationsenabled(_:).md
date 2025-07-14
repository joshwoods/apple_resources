

- UIKit
- UIView
-  setAnimationsEnabled(\_:) 

Type Method

# setAnimationsEnabled(\_:)

Sets whether animations are enabled.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
class func setAnimationsEnabled(_ enabled: Bool)
```

## Parameters 

`enabled`  

Specify true to enable animations or false to disable them.

## Discussion

Animations are enabled by default. If you disable animations, code inside subsequent animation blocks is still executed but no animations actually occur. Thus, any changes you make inside an animation block are reflected immediately instead of being animated. This is true whether you use the block-based animation methods or the begin/commit animation methods.

This method affects only those animations that are submitted after it is called. If you call this method while existing animations are running, those animations continue running until they reach their natural end point.

## See Also

### Related Documentation

class func performWithoutAnimation(() -> Void)

Disables a view transition animation.

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

