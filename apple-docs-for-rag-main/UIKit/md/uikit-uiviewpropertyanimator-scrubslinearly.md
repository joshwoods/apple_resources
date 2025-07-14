

- UIKit
- UIViewPropertyAnimator
-  scrubsLinearly 

Instance Property

# scrubsLinearly

A Boolean value indicating whether a paused animation scrubs linearly or uses its specified timing information.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var scrubsLinearly: Bool { get set }
```

## Discussion

The default value of this property is true, which causes the animator to use a linear timing function during scrubbing. Setting the property to false causes the animator to use its specified timing curve.

## See Also

### Accessing the animation parameters

var duration: TimeInterval

The total duration (in seconds) of the main animations.

var delay: TimeInterval

The delay (in seconds) after which the animations begin.

var timingParameters: (any UITimingCurveProvider)?

The information used to determine the timing curve for the animation.

var isInterruptible: Bool

A Boolean value indicating whether the animator is interruptible and can be paused or stopped.

var isUserInteractionEnabled: Bool

A Boolean value indicating whether views receive touch events while animations are running.

var isManualHitTestingEnabled: Bool

A Boolean value indicating whether your app manages hit-testing while animations are in progress.

var pausesOnCompletion: Bool

A Boolean value that indicates whether a completed animation remains in the active state.

