

- AppKit
- NSGestureRecognizer
-  isEnabled 

Instance Property

# isEnabled

A Boolean value indicating whether the gesture recognizer is able to handle events.

macOS 10.10+

``` source
@MainActor
var isEnabled: Bool { get set }
```

## Discussion

When the value of this property is true, the gesture recognizer receives events and uses them to determine when its gesture is performed. When the value is false, the gesture recognizer does not receive events. Changing the value from true to false while the gesture recognizer is in the process of recognizing a gesture changes the state of the gesture recognizer to NSGestureRecognizer.State.cancelled.

The default value of this property is true.

## See Also

### Accessing the Recognizer’s State

var state: NSGestureRecognizer.State

The current state of the gesture recognizer.

var view: NSView?

The view to which the gesture recognizer is attached.

