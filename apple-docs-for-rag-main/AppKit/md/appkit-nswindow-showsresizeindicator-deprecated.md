

- AppKit
- NSWindow
-  showsResizeIndicator Deprecated

Instance Property

# showsResizeIndicator

A Boolean value that indicates whether the window’s resize indicator is visible.

macOS 10.0–15.0Deprecated

``` source
@MainActor
var showsResizeIndicator: Bool { get set }
```

Deprecated

This property does not do anything and should not be used.

## Discussion

The value of this property is true when the window’s resize indicator is visible; otherwise, false. This property does not affect whether the window is resizable.

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

var isFlushWindowDisabled: Bool

A Boolean value that indicates whether the window’s flushing ability is disabled.

Deprecated

var isAutodisplay: Bool

A Boolean value that indicates whether the window automatically displays views that need to be displayed.

Deprecated

var graphicsContext: NSGraphicsContext?

The graphics context associated with the window for the current thread.

Deprecated

var windowRef: UnsafeMutableRawPointer

The Carbon window reference associated with the window, creating one if necessary.

Deprecated

