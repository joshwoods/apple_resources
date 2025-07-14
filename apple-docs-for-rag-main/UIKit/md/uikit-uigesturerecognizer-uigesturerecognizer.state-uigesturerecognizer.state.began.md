

- UIKit
- UIGestureRecognizer
- UIGestureRecognizer.State
-  UIGestureRecognizer.State.began 

Case

# UIGestureRecognizer.State.began

The gesture recognizer has received touch objects recognized as a continuous gesture.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
case began
```

## Mentioned in 

About the Gesture Recognizer State Machine

Handling long-press gestures

Handling rotation gestures

Handling pinch gestures

Handling pan gestures

## Discussion

The gesture recognizer sends its action message (or messages) at the next cycle of the run loop.

## See Also

### Constants

case possible

The gesture recognizer hasn’t yet recognized its gesture, but may be evaluating touch events.

case changed

The gesture recognizer has received touches recognized as a change to a continuous gesture.

case ended

The gesture recognizer has received touches recognized as the end of a continuous gesture.

case cancelled

The gesture recognizer has received touches resulting in the cancellation of a continuous gesture.

case failed

The gesture recognizer has received a multi-touch sequence that it can’t recognize as its gesture.

static var recognized: UIGestureRecognizer.State

The gesture recognizer has received a multitouch sequence that it recognizes as its gesture.

