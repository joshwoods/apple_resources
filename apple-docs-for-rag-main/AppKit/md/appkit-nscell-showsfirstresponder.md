

- AppKit
- NSCell
-  showsFirstResponder 

Instance Property

# showsFirstResponder

A Boolean value indicating whether the cell provides a visual indication that it is the first responder.

macOS

``` source
@MainActor
var showsFirstResponder: Bool { get set }
```

## Discussion

When the value of this property is true and the cell becomes the first responder, the cell performs additional drawing to indicate that it is the first responder. The `NSCell` class itself does not draw a first-responder indicator. Subclasses may use the value in this property to determine whether or not they should draw one.

## See Also

### Respond to Keyboard Events

var acceptsFirstResponder: Bool

A Boolean value indicating whether the cell accepts first responder status.

var refusesFirstResponder: Bool

A Boolean value indicating whether the cell refuses the first responder status.

func performClick(Any?)

Simulates a single mouse click on the receiver.

