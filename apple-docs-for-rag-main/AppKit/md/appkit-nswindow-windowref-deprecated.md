

- AppKit
- NSWindow
-  windowRef Deprecated

Instance Property

# windowRef

The Carbon window reference associated with the window, creating one if necessary.

macOS 10.0–15.0Deprecated

``` source
@MainActor
var windowRef: UnsafeMutableRawPointer { get }
```

Deprecated

This method should not be used.

## Discussion

You can use this property to create a `WindowRef` for a window containing a Carbon control. Subsequent accesses to this property get the existing `WindowRef`. You use a `WindowRef` to create a Carbon window reference for a Cocoa window; this assists the integration of Carbon and Cocoa code and objects.

For more information see the `MacWindows.h` header file.

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

var graphicsContext: NSGraphicsContext?

The graphics context associated with the window for the current thread.

Deprecated

