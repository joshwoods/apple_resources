

- UIKit
- UIGestureRecognizer
- UIGestureRecognizer.State
-  UIGestureRecognizer.State.failed 

Case

# UIGestureRecognizer.State.failed

The gesture recognizer has received a multi-touch sequence that it can’t recognize as its gesture.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
case failed
```

## Mentioned in 

About the Gesture Recognizer State Machine

## Discussion

No action message is sent and the gesture recognizer is reset to UIGestureRecognizer.State.possible.

## See Also

### Constants

case possible

The gesture recognizer hasn’t yet recognized its gesture, but may be evaluating touch events.

case began

The gesture recognizer has received touch objects recognized as a continuous gesture.

case changed

The gesture recognizer has received touches recognized as a change to a continuous gesture.

case ended

The gesture recognizer has received touches recognized as the end of a continuous gesture.

case cancelled

The gesture recognizer has received touches resulting in the cancellation of a continuous gesture.

static var recognized: UIGestureRecognizer.State

The gesture recognizer has received a multitouch sequence that it recognizes as its gesture.

