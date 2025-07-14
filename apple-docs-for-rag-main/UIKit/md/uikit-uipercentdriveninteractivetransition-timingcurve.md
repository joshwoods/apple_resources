

- UIKit
- UIPercentDrivenInteractiveTransition
-  timingCurve 

Instance Property

# timingCurve

The timing curve to use when driving the animations.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
var timingCurve: (any UITimingCurveProvider)? { get set }
```

## See Also

### Accessing transition attributes

var completionCurve: UIView.AnimationCurve

Indicates the animation completion curve for an interactive transition.

var duration: CGFloat

The overall duration (in seconds) of the transition animation.

var percentComplete: CGFloat

The amount of the transition (specified as a percentage of the overall duration) that’s complete.

var completionSpeed: CGFloat

The speed of the transition animation.

var wantsInteractiveStart: Bool

A Boolean value indicating whether the animations are interactive initially.

