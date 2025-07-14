

- AppKit
- NSCell
-  performClick(\_:) 

Instance Method

# performClick(\_:)

Simulates a single mouse click on the receiver.

macOS

``` source
@MainActor
func performClick(_ sender: Any?)
```

## Parameters 

`sender`  

The object to use as the sender of the event (if the receiver’s control view is not valid). This object must be a subclass of `NSView`.

## Discussion

This method performs the receiver’s action on its target. The receiver must be enabled to perform the action. If the receiver’s control view is valid, that view is used as the sender; otherwise, the value in `sender` is used.

The receiver of this message must be a cell of type `NSActionCell`. This method raises an exception if the action message cannot be successfully sent.

## See Also

### Related Documentation

var controlView: NSView?

The view associated with the cell.

### Respond to Keyboard Events

var acceptsFirstResponder: Bool

A Boolean value indicating whether the cell accepts first responder status.

var showsFirstResponder: Bool

A Boolean value indicating whether the cell provides a visual indication that it is the first responder.

var refusesFirstResponder: Bool

A Boolean value indicating whether the cell refuses the first responder status.

