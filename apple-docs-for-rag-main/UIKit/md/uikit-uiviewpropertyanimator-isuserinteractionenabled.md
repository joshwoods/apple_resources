

- UIKit
- UIViewPropertyAnimator
-  isUserInteractionEnabled 

Instance Property

# isUserInteractionEnabled

A Boolean value indicating whether views receive touch events while animations are running.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
var isUserInteractionEnabled: Bool { get set }
```

## Discussion

When the value of this property is true, touch events are delivered to views normally. Setting this property to false causes touch events to be ignored in animated views for the duration of the animations. The default value of this property is true.

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

var isManualHitTestingEnabled: Bool

A Boolean value indicating whether your app manages hit-testing while animations are in progress.

var scrubsLinearly: Bool

A Boolean value indicating whether a paused animation scrubs linearly or uses its specified timing information.

var pausesOnCompletion: Bool

A Boolean value that indicates whether a completed animation remains in the active state.

