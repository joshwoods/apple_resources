

- AppKit
- NSView
-  canBecomeKeyView 

Instance Property

# canBecomeKeyView

A Boolean value indicating whether the view can become key view.

macOS

``` source
@MainActor
var canBecomeKeyView: Bool { get }
```

## Discussion

When the value of this property is true, the view can become the key view. In order to become the key view, the view must be visible, it must be installed in a window that supports keyboard entry, and the view’s acceptsFirstResponder method must return true.

## See Also

### Managing the Key-View Loop

var needsPanelToBecomeKey: Bool

A Boolean value indicating whether the view needs its panel to become the key window before it can handle keyboard input and navigation.

var nextKeyView: NSView?

The view object that follows the current view in the key view loop.

var nextValidKeyView: NSView?

The closest view object in the key view loop that follows the current view in the key view loop and accepts first responder status.

var previousKeyView: NSView?

The view object preceding the current view in the key view loop.

var previousValidKeyView: NSView?

The closest view object in the key view loop that precedes the current view and accepts first responder status.

