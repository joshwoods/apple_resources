

- UIKit
- UIViewPropertyAnimator
-  isInterruptible 

Instance Property

# isInterruptible

A Boolean value indicating whether the animator is interruptible and can be paused or stopped.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
var isInterruptible: Bool { get set }
```

## Discussion

When the value of this property is true, you can use the pauseAnimation() and stopAnimation(_:) methods to interrupt the animations and make changes. When the value of this property is false, the animations run to completion (and without interruption) after you call the startAnimation() method. If you use a view property animator object to implement an interruptible view controller transition, this property must be true.

It is a programmer error to change this property if the animator’s state property is not set to UIViewAnimatingState.inactive.

## See Also

### Accessing the animation parameters

var duration: TimeInterval

The total duration (in seconds) of the main animations.

var delay: TimeInterval

The delay (in seconds) after which the animations begin.

var timingParameters: (any UITimingCurveProvider)?

The information used to determine the timing curve for the animation.

var isUserInteractionEnabled: Bool

A Boolean value indicating whether views receive touch events while animations are running.

var isManualHitTestingEnabled: Bool

A Boolean value indicating whether your app manages hit-testing while animations are in progress.

var scrubsLinearly: Bool

A Boolean value indicating whether a paused animation scrubs linearly or uses its specified timing information.

var pausesOnCompletion: Bool

A Boolean value that indicates whether a completed animation remains in the active state.

