

- UIKit
- UIView
-  setAnimationWillStart(\_:) Deprecated

Type Method

# setAnimationWillStart(\_:)

Sets the message to send to the animation delegate when the animation starts.

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
class func setAnimationWillStart(_ selector: Selector?)
```

## Parameters 

`selector`  

The message to send to the animation delegate before animations start. The default value is `NULL`. This selector should be of the form: `- (void)animationDidStart:(NSString *)animationID context:(void *)context`. Your method must take the following arguments:

- `animationID`

An NSString containing an optional application-supplied identifier. This is the identifier string that is passed to the beginAnimations(_:context:) method. This argument can be `nil`.

- `context`

An optional application-supplied context. This is the context data passed to the beginAnimations(_:context:) method. This argument can be `nil`.

## Discussion

If you specify an animation delegate for a begin/commit set of animations, you use this method to specify the selector to call before the animations begin. This method does nothing if called from outside of an animation block. It must be called between calls to the beginAnimations(_:context:) and commitAnimations() methods. This selector is set to `NULL` by default.

Note

Your start selector is not called if animations are disabled.

Use of this method is discouraged in iOS 4.0 and later. If you are using the block-based animation methods, you can include your delegate’s start code directly inside your block.

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

