

- UIKit
- UIPercentDrivenInteractiveTransition
-  completionCurve 

Instance Property

# completionCurve

Indicates the animation completion curve for an interactive transition.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var completionCurve: UIView.AnimationCurve { get set }
```

## Discussion

When the interactive part of a view controller transition is complete, you can set this property to indicate a desired animation completion curve. Default value is UIView.AnimationCurve.easeInOut.

During the interactive portion of a view controller transition, the animation curve is linear.

## See Also

### Accessing transition attributes

var timingCurve: (any UITimingCurveProvider)?

The timing curve to use when driving the animations.

var duration: CGFloat

The overall duration (in seconds) of the transition animation.

var percentComplete: CGFloat

The amount of the transition (specified as a percentage of the overall duration) that’s complete.

var completionSpeed: CGFloat

The speed of the transition animation.

var wantsInteractiveStart: Bool

A Boolean value indicating whether the animations are interactive initially.

