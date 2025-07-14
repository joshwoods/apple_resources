

- UIKit
- Views and controls
- UIView
-  Deprecated symbols 

API Collection

# Deprecated symbols

Symbols that views no longer support.

## Topics

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

class func setAnimationTransition(UIView.AnimationTransition, for: UIView, cache: Bool)

Sets a transition to apply to a view during an animation block.

Deprecated

class var areAnimationsEnabled: Bool

Returns a Boolean value indicating whether animations are enabled.

func forBaselineLayout() -> UIView

Returns a view used to satisfy baseline constraints.

Deprecated

