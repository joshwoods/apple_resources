

- AppKit
- NSResponder
-  becomeFirstResponder() 

Instance Method

# becomeFirstResponder()

Notifies the receiver that it’s about to become first responder in its NSWindow.

macOS

``` source
@MainActor
func becomeFirstResponder() -> Bool
```

## Discussion

The default implementation returns true, accepting first responder status. Subclasses can override this method to update state or perform some action such as highlighting the selection, or to return false, refusing first responder status.

Use the `NSWindow` makeFirstResponder(_:) method, not this method, to make an object the first responder. Never invoke this method directly.

## See Also

### Changing the First Responder

var acceptsFirstResponder: Bool

A Boolean value that indicates whether the responder accepts first responder status.

func resignFirstResponder() -> Bool

Notifies the receiver that it’s been asked to relinquish its status as first responder in its window.

func validateProposedFirstResponder(NSResponder, for: NSEvent?) -> Bool

Allows controls to determine when they should become first responder.

