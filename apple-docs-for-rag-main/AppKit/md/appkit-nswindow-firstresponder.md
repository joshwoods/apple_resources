

- AppKit
- NSWindow
-  firstResponder 

Instance Property

# firstResponder

The window’s first responder.

macOS

``` source
@MainActor
weak var firstResponder: NSResponder? { get }
```

## Discussion

The first responder is usually the first object in a responder chain to receive an event or action message. In most cases, the first responder is a view object that the user selects or activates with the mouse or keyboard.

You can use the firstResponder property in custom subclasses of responder classes (NSWindow, NSApplication, NSView, and subclasses) to determine if an instance of the subclass is currently the first responder. You can also use it to help locate a text field that currently has first-responder status. For more on this subject, see Event Handling Basics. This property is key-value observing compliant.

## See Also

### Related Documentation

var acceptsFirstResponder: Bool

A Boolean value that indicates whether the responder accepts first responder status.

### Managing Responders

var initialFirstResponder: NSView?

The view that’s made first responder (also called the key view) the first time the window is placed onscreen.

func makeFirstResponder(NSResponder?) -> Bool

Attempts to make a given responder the first responder for the window.

