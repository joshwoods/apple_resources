

- AppKit
- NSCell
-  refusesFirstResponder 

Instance Property

# refusesFirstResponder

A Boolean value indicating whether the cell refuses the first responder status.

macOS

``` source
@MainActor
var refusesFirstResponder: Bool { get set }
```

## Discussion

Set the value of this property to true to prevent the cell from becoming the first responder. To determine whether the cell can become first responder right now, get the value of the acceptsFirstResponder property.

## See Also

### Respond to Keyboard Events

var acceptsFirstResponder: Bool

A Boolean value indicating whether the cell accepts first responder status.

var showsFirstResponder: Bool

A Boolean value indicating whether the cell provides a visual indication that it is the first responder.

func performClick(Any?)

Simulates a single mouse click on the receiver.

