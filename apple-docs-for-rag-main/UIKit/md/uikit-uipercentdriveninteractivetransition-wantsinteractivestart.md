

- UIKit
- UIPercentDrivenInteractiveTransition
-  wantsInteractiveStart 

Instance Property

# wantsInteractiveStart

A Boolean value indicating whether the animations are interactive initially.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
var wantsInteractiveStart: Bool { get set }
```

## Discussion

When the value of this property is true, interactive animations start as paused, allowing you to drive the animations yourself from the start. You might set this property to false when you want to start your animations without interactivity. The default value of this property is true.

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

var completionSpeed: CGFloat

The speed of the transition animation.

