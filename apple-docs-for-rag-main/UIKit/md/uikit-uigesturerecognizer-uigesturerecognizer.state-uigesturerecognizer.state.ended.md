

- UIKit
- UIGestureRecognizer
- UIGestureRecognizer.State
-  UIGestureRecognizer.State.ended 

Case

# UIGestureRecognizer.State.ended

The gesture recognizer has received touches recognized as the end of a continuous gesture.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
case ended
```

## Mentioned in 

About the Gesture Recognizer State Machine

Implementing a Continuous Gesture Recognizer

Handling rotation gestures

Handling long-press gestures

Handling pan gestures

## Discussion

The gesture recognizer sends its action message (or messages) at the next cycle of the run loop and resets its state to UIGestureRecognizer.State.possible.

## See Also

### Constants

case possible

The gesture recognizer hasn’t yet recognized its gesture, but may be evaluating touch events.

case began

The gesture recognizer has received touch objects recognized as a continuous gesture.

case changed

The gesture recognizer has received touches recognized as a change to a continuous gesture.

case cancelled

The gesture recognizer has received touches resulting in the cancellation of a continuous gesture.

case failed

The gesture recognizer has received a multi-touch sequence that it can’t recognize as its gesture.

static var recognized: UIGestureRecognizer.State

The gesture recognizer has received a multitouch sequence that it recognizes as its gesture.

