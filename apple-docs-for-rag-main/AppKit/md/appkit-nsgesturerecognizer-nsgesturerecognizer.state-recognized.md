

- AppKit
- NSGestureRecognizer
- NSGestureRecognizer.State
-  recognized 

Type Property

# recognized

The gesture recognizer successfully recognized its gesture. It calls its action method at the next cycle of the run loop and resets its state to NSGestureRecognizer.State.possible.

macOS 10.10+

``` source
static var recognized: NSGestureRecognizer.State { get }
```

## See Also

### Constants

case possible

The gesture recognizer has not yet recognized its gesture but may be evaluating events. This is the default state.

case began

The gesture recognizer has recognized a sequence of events as a continuous gesture. It calls its action method at the next cycle of the run loop.

case changed

The gesture recognizer has detected a change to a continuous gesture. It calls its action method at the next cycle of the run loop.

case ended

The gesture recognizer has detected the end of a continuous gesture. It calls its action method at the next cycle of the run loop and resets its state to NSGestureRecognizer.State.possible.

case cancelled

The gesture recognizer received events that resulted in the cancellation of a continuous gesture. It calls its action method at the next cycle of the run loop and resets its state to NSGestureRecognizer.State.possible.

case failed

The gesture recognizer failed to recognize its gesture and will not call its action method. The gesture recognizer resets itself to the NSGestureRecognizer.State.possible state.

