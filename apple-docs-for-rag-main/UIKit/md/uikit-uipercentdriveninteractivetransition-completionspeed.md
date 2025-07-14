

- UIKit
- UIPercentDrivenInteractiveTransition
-  completionSpeed 

Instance Property

# completionSpeed

The speed of the transition animation.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var completionSpeed: CGFloat { get set }
```

## Discussion

The default value of this property is `1.0`, which yields an animation that proceeds in real time. You typically change this value to speed up or slow down the animation at specific points in the transition. For example, you might change the animation speed at the end of a transition or when canceling it, in which case you would set the speed when you stop tracking user events and are about to call the cancel() or finish() method.

The speed acts as a multiplier to the current animation speed, so values greater than `1.0` speed up the animation and values less than `1.0` slow it down. The value in this property must always be greater than `0.0`.

## See Also

### Accessing transition attributes

var timingCurve: (any UITimingCurveProvider)?

The timing curve to use when driving the animations.

var completionCurve: UIView.AnimationCurve

Indicates the animation completion curve for an interactive transition.

var duration: CGFloat

The overall duration (in seconds) of the transition animation.

var percentComplete: CGFloat

The amount of the transition (specified as a percentage of the overall duration) that’s complete.

var wantsInteractiveStart: Bool

A Boolean value indicating whether the animations are interactive initially.

