

- AppKit
- NSWindow
-  isOneShot Deprecated

Instance Property

# isOneShot

A Boolean value that indicates whether the window device the window manages is freed when it’s removed from the screen list.

macOS 10.0–10.14Deprecated

``` source
@MainActor
var isOneShot: Bool { get set }
```

Deprecated

This property does not do anything and should not be used

## Discussion

When the value of this property is true, the window’s window device is freed when it’s removed from the screen list (that is, hidden) and another is created when it’s returned to the screen. When the value is false, the window device is reused. Freeing the window device when it’s removed from the screen list can result in memory savings and performance improvement for window objects that don’t take long to display. Doing so is particularly appropriate for window objects the user might use once or twice, but not display continually.

## See Also

### Properties

var backingLocation: NSWindow.BackingLocation

The location of the window’s backing store.

Deprecated

var preferredBackingLocation: NSWindow.BackingLocation

A Boolean value that indicates the preferred location for the window’s backing store.

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

var graphicsContext: NSGraphicsContext?

The graphics context associated with the window for the current thread.

Deprecated

var windowRef: UnsafeMutableRawPointer

The Carbon window reference associated with the window, creating one if necessary.

Deprecated

