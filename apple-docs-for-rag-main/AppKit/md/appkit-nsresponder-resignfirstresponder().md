

- AppKit
- NSResponder
-  resignFirstResponder() 

Instance Method

# resignFirstResponder()

Notifies the receiver that it’s been asked to relinquish its status as first responder in its window.

macOS

``` source
@MainActor
func resignFirstResponder() -> Bool
```

## Discussion

The default implementation returns true, resigning first responder status. Subclasses can override this method to update state or perform some action such as unhighlighting the selection, or to return false, refusing to relinquish first responder status.

Use the `NSWindow` makeFirstResponder(_:) method, not this method, to make an object the first responder. Never invoke this method directly.

## See Also

### Changing the First Responder

var acceptsFirstResponder: Bool

A Boolean value that indicates whether the responder accepts first responder status.

func becomeFirstResponder() -> Bool

Notifies the receiver that it’s about to become first responder in its NSWindow.

func validateProposedFirstResponder(NSResponder, for: NSEvent?) -> Bool

Allows controls to determine when they should become first responder.

