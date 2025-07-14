

- AppKit
- NSResponder
-  acceptsFirstResponder 

Instance Property

# acceptsFirstResponder

A Boolean value that indicates whether the responder accepts first responder status.

macOS

``` source
@MainActor
var acceptsFirstResponder: Bool { get }
```

## Discussion

As first responder, the receiver is the first object in the responder chain to be sent key events and action messages. By default, this property is false. Subclasses set this property to true if the receiver accepts first responder status.

## See Also

### Related Documentation

var needsPanelToBecomeKey: Bool

A Boolean value indicating whether the view needs its panel to become the key window before it can handle keyboard input and navigation.

Cocoa Event Handling Guide

### Changing the First Responder

func becomeFirstResponder() -> Bool

Notifies the receiver that it’s about to become first responder in its NSWindow.

func resignFirstResponder() -> Bool

Notifies the receiver that it’s been asked to relinquish its status as first responder in its window.

func validateProposedFirstResponder(NSResponder, for: NSEvent?) -> Bool

Allows controls to determine when they should become first responder.

