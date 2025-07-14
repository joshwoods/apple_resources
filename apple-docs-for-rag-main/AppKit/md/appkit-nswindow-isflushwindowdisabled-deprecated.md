

- AppKit
- NSWindow
-  isFlushWindowDisabled Deprecated

Instance Property

# isFlushWindowDisabled

A Boolean value that indicates whether the window’s flushing ability is disabled.

macOS 10.0–10.14Deprecated

``` source
@MainActor
var isFlushWindowDisabled: Bool { get }
```

Deprecated

Use +\[NSAnimationContext runAnimationGroup:completionHandler:\] to perform atomic updates across runloop invocations.

## Discussion

The value of this property is true when the window’s flushing ability has been disabled; otherwise, false.

## See Also

### Related Documentation

func disableFlushing()

Disables the flush() method for the window.

Deprecated

func enableFlushing()

Reenables the flush() method for the window after it was disabled through a previous disableFlushing() message.

Deprecated

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

var isAutodisplay: Bool

A Boolean value that indicates whether the window automatically displays views that need to be displayed.

Deprecated

var graphicsContext: NSGraphicsContext?

The graphics context associated with the window for the current thread.

Deprecated

var windowRef: UnsafeMutableRawPointer

The Carbon window reference associated with the window, creating one if necessary.

Deprecated

