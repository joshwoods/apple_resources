

- AppKit
- NSControl
-  mouseDown(with:) 

Instance Method

# mouseDown(with:)

Informs the receiver that the user has pressed the left mouse button.

macOS

``` source
@MainActor
func mouseDown(with event: NSEvent)
```

## Parameters 

`event`  

The event resulting from the user action.

## Discussion

Invoked when the mouse button is pressed while the cursor is within the bounds of the receiver, generating `theEvent`. This method highlights the receiver’s cell and sends it a trackMouse(with:in:of:untilMouseUp:) message. Whenever the cell finishes tracking the mouse (for example, because the cursor has left the cell’s bounds), the cell is unhighlighted. If the mouse button is still down and the cursor reenters the bounds, the cell is again highlighted and a new trackMouse(with:in:of:untilMouseUp:) message is sent. This behavior repeats until the mouse button goes up. If it goes up with the cursor in the control, the state of the control is changed, and the action message is sent to the target. If the mouse button goes up when the cursor is outside the control, no action message is sent.

## See Also

### Related Documentation

func trackMouse(with: NSEvent, in: NSRect, of: NSView, untilMouseUp: Bool) -> Bool

Initiates the mouse tracking behavior in a cell.

### Tracking the Mouse

var ignoresMultiClick: Bool

A Boolean value indicating whether the receiver ignores multiple clicks made in rapid succession.

