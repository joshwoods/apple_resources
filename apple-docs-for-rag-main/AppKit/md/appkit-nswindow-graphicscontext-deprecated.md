

- AppKit
- NSWindow
-  graphicsContext Deprecated

Instance Property

# graphicsContext

The graphics context associated with the window for the current thread.

macOS 10.0–10.14Deprecated

``` source
@MainActor
var graphicsContext: NSGraphicsContext? { get }
```

Deprecated

Add instances of NSView to display content in a window.

## See Also

### Properties

var backingLocation: NSWindow.BackingLocation

The location of the window’s backing store.

Deprecated

var preferredBackingLocation: NSWindow.BackingLocation

A Boolean value that indicates the preferred location for the window’s backing store.

Deprecated

var isOneShot: Bool

A Boolean value that indicates whether the window device the window manages is freed when it’s removed from the screen list.

Deprecated

var drawers: [NSDrawer]?

The collection of drawers associated with the window.

Deprecated

var showsResizeIndicator: Bool

A Boolean value that indicates whether the window’s resize indicator is visible.

Deprecated

var isFlushWindowDisabled: Bool

A Boolean value that indicates whether the window’s flushing ability is disabled.

Deprecated

var isAutodisplay: Bool

A Boolean value that indicates whether the window automatically displays views that need to be displayed.

Deprecated

var windowRef: UnsafeMutableRawPointer

The Carbon window reference associated with the window, creating one if necessary.

Deprecated

