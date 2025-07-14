

- AppKit
- NSResponder
-  validateProposedFirstResponder(\_:for:) 

Instance Method

# validateProposedFirstResponder(\_:for:)

Allows controls to determine when they should become first responder.

macOS 10.7+

``` source
@MainActor
func validateProposedFirstResponder(
    _ responder: NSResponder,
    for event: NSEvent?
) -> Bool
```

## Parameters 

`responder`  

The first responder.

`event`  

The event to validate. May be `nil` if there is no applicable event.

## Return Value

true if the control should become first responder, otherwise false.

## Discussion

Some controls, such as `NSTextField`, should only become first responder when the enclosing NSTableView/NSBrowser indicates that the view can begin editing. It is up to the particular control that wants to be validated to call this method in its mouseDown(with:) method (or perhaps at another time) to determine if it should attempt to become the first responder or not.

The NSTableView, NSOutlineView, and NSBrowser classes implement this to allow first responder status only if the responder is a view in a selected row. It also delays the first responder assignment if a `doubleAction` may be invoked.

The default implementation returns true when there is no nextResponder set, otherwise, it is forwarded up the responder chain.

## See Also

### Changing the First Responder

var acceptsFirstResponder: Bool

A Boolean value that indicates whether the responder accepts first responder status.

func becomeFirstResponder() -> Bool

Notifies the receiver that it’s about to become first responder in its NSWindow.

func resignFirstResponder() -> Bool

Notifies the receiver that it’s been asked to relinquish its status as first responder in its window.

