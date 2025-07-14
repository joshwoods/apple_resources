

- AppKit
- NSCell
-  acceptsFirstResponder 

Instance Property

# acceptsFirstResponder

A Boolean value indicating whether the cell accepts first responder status.

macOS

``` source
@MainActor
var acceptsFirstResponder: Bool { get }
```

## Discussion

When the value of this property is true, the cell is able to become the first responder. The default value of this property is true when the cell is enabled. Subclasses may override this method to return a different value.

## See Also

### Respond to Keyboard Events

var showsFirstResponder: Bool

A Boolean value indicating whether the cell provides a visual indication that it is the first responder.

var refusesFirstResponder: Bool

A Boolean value indicating whether the cell refuses the first responder status.

func performClick(Any?)

Simulates a single mouse click on the receiver.

