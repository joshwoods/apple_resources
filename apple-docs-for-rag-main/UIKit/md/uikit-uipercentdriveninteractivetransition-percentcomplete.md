

- UIKit
- UIPercentDrivenInteractiveTransition
-  percentComplete 

Instance Property

# percentComplete

The amount of the transition (specified as a percentage of the overall duration) that’s complete.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var percentComplete: CGFloat { get }
```

## Discussion

The value in this property reflects the last value passed to the update(_:) method.

## See Also

### Related Documentation

func update(CGFloat)

Updates the completion percentage of the transition.

### Accessing transition attributes

var timingCurve: (any UITimingCurveProvider)?

The timing curve to use when driving the animations.

var completionCurve: UIView.AnimationCurve

Indicates the animation completion curve for an interactive transition.

var duration: CGFloat

The overall duration (in seconds) of the transition animation.

var completionSpeed: CGFloat

The speed of the transition animation.

var wantsInteractiveStart: Bool

A Boolean value indicating whether the animations are interactive initially.

