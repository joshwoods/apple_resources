

- UIKit
- UIGestureRecognizer
- UIGestureRecognizer.State
-  UIGestureRecognizer.State.possible 

Case

# UIGestureRecognizer.State.possible

The gesture recognizer hasn’t yet recognized its gesture, but may be evaluating touch events.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
case possible
```

## Mentioned in 

About the Gesture Recognizer State Machine

Implementing a Discrete Gesture Recognizer

## Discussion

This is the default state.

## See Also

### Constants

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

static var recognized: UIGestureRecognizer.State

The gesture recognizer has received a multitouch sequence that it recognizes as its gesture.

