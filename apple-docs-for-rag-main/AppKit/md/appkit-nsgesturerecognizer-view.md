

- AppKit
- NSGestureRecognizer
-  view 

Instance Property

# view

The view to which the gesture recognizer is attached.

macOS 10.10+

``` source
@MainActor
var view: NSView? { get }
```

## Discussion

To attach a gesture recognizer to a view, call the addGestureRecognizer(_:) method of the view. If the gesture recognizer is not attached to a view, the value in this property is `nil`.

## See Also

### Related Documentation

func location(in: NSView?) -> NSPoint

Returns the point computed as the location of the gesture.

### Accessing the Recognizer’s State

var state: NSGestureRecognizer.State

The current state of the gesture recognizer.

var isEnabled: Bool

A Boolean value indicating whether the gesture recognizer is able to handle events.

