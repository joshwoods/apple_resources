

- AppKit
- NSWindow
-  isAutodisplay Deprecated

Instance Property

# isAutodisplay

A Boolean value that indicates whether the window automatically displays views that need to be displayed.

macOS 10.0–10.14Deprecated

``` source
@MainActor
var isAutodisplay: Bool { get set }
```

Deprecated

Use +\[NSAnimationContext runAnimationGroup:completionHandler:\] to temporarily prevent AppKit's automatic deferred display mechanism from drawing.

## Discussion

The value of this property is true when the window automatically displays views that need to be displayed; otherwise, false. If `autodisplay` is false, the window or its views must be explicitly displayed.

Automatic display typically occurs on each pass through the event loop.

## See Also

### Related Documentation

var needsDisplay: Bool

A Boolean value that determines whether the view needs to be redrawn before being displayed.

func displayIfNeeded()

Passes a display message down the window’s view hierarchy, thus redrawing all views that need displaying.

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

var graphicsContext: NSGraphicsContext?

The graphics context associated with the window for the current thread.

Deprecated

var windowRef: UnsafeMutableRawPointer

The Carbon window reference associated with the window, creating one if necessary.

Deprecated

