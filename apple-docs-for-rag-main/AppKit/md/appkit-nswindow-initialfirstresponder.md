

- AppKit
- NSWindow
-  initialFirstResponder 

Instance Property

# initialFirstResponder

The view that’s made first responder (also called the key view) the first time the window is placed onscreen.

macOS

``` source
@MainActor
weak var initialFirstResponder: NSView? { get set }
```

## See Also

### Related Documentation

var nextKeyView: NSView?

The view object that follows the current view in the key view loop.

### Managing Responders

var firstResponder: NSResponder?

The window’s first responder.

func makeFirstResponder(NSResponder?) -> Bool

Attempts to make a given responder the first responder for the window.

