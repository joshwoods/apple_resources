

- UIKit
- UIViewPropertyAnimator
-  duration 

Instance Property

# duration

The total duration (in seconds) of the main animations.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
var duration: TimeInterval { get }
```

## Discussion

You set the duration value when creating the animator and cannot change it later. Animations added while the animator is in the inactive state are run for the specified duration. Animations added later run only for the remaining time, which is determined by the formula `(1.0 - fractionComplete) * duration`.

## See Also

### Accessing the animation parameters

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

var scrubsLinearly: Bool

A Boolean value indicating whether a paused animation scrubs linearly or uses its specified timing information.

var pausesOnCompletion: Bool

A Boolean value that indicates whether a completed animation remains in the active state.

