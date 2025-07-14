

- AppKit
- NSGestureRecognizer
-  state 

Instance Property

# state

The current state of the gesture recognizer.

macOS 10.10+

``` source
@MainActor
var state: NSGestureRecognizer.State { get set }
```

## Discussion

This property conveys where the gesture recognizer is in the recognition process. The default declaration of this property is read-only so that external clients (such as other gesture recognizers) can use the value for informational purposes. Subclasses can redeclare the property as read-write internally. When doing so, you do not need to provide a custom implementation to set the value of the property. This class provides an implementation that detects state transitions and updates the gesture recognizer accordingly.

For more information about the state transitions that can occur in a gesture recognizer, see State Transitions.

## See Also

### Accessing the Recognizer’s State

var view: NSView?

The view to which the gesture recognizer is attached.

var isEnabled: Bool

A Boolean value indicating whether the gesture recognizer is able to handle events.

