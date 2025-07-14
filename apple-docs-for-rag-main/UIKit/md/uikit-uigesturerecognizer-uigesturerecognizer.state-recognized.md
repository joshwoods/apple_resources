

- UIKit
- UIGestureRecognizer
- UIGestureRecognizer.State
-  recognized 

Type Property

# recognized

The gesture recognizer has received a multitouch sequence that it recognizes as its gesture.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
static var recognized: UIGestureRecognizer.State { get }
```

## Mentioned in 

Implementing a Discrete Gesture Recognizer

Implementing a Continuous Gesture Recognizer

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

case ended

The gesture recognizer has received touches recognized as the end of a continuous gesture.

case cancelled

The gesture recognizer has received touches resulting in the cancellation of a continuous gesture.

case failed

The gesture recognizer has received a multi-touch sequence that it can’t recognize as its gesture.

