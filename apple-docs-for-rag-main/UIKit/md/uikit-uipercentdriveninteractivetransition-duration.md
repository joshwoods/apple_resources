

- UIKit
- UIPercentDrivenInteractiveTransition
-  duration 

Instance Property

# duration

The overall duration (in seconds) of the transition animation.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var duration: CGFloat { get }
```

## Discussion

This property reflects the duration of the transition animation if it were to occur without user interactions. It is obtained from the standard animator object returned by your delegate. The actual duration can vary depending on the user interactions you are tracking and responding to.

## See Also

### Related Documentation

func transitionDuration(using: (any UIViewControllerContextTransitioning)?) -> TimeInterval

Asks your animator object for the duration (in seconds) of the transition animation.

**Required**

### Accessing transition attributes

var timingCurve: (any UITimingCurveProvider)?

The timing curve to use when driving the animations.

var completionCurve: UIView.AnimationCurve

Indicates the animation completion curve for an interactive transition.

var percentComplete: CGFloat

The amount of the transition (specified as a percentage of the overall duration) that’s complete.

var completionSpeed: CGFloat

The speed of the transition animation.

var wantsInteractiveStart: Bool

A Boolean value indicating whether the animations are interactive initially.

