

- AppKit
- NSToolbar
-  fullScreenAccessoryView Deprecated

Instance Property

# fullScreenAccessoryView

The toolbar’s full screen accessory view.

macOS 10.7–10.13Deprecated

``` source
@MainActor
var fullScreenAccessoryView: NSView? { get set }
```

Deprecated

Use an NSTitlebarAccessoryViewController with an NSWindow instead.

## Discussion

When entering full screen mode, the accessory view is removed from the window if necessary, and attaches underneath the toolbar.

When leaving full screen mode, the accessory view is returned to the window, if it was in the window previously.

To customize this behavior, you can implement the NSWindow delegate method windowWillExitFullScreen(_:).

## See Also

### Deprecated

var centeredItemIdentifier: NSToolbarItem.Identifier?

The item to display in the center of the toolbar.

Deprecated

var fullScreenAccessoryViewMinHeight: CGFloat

The minimum height of the toolbar’s full screen accessory view.

Deprecated

var fullScreenAccessoryViewMaxHeight: CGFloat

The maximum height of the toolbar’s full screen accessory view, in points.

Deprecated

var sizeMode: NSToolbar.SizeMode

The toolbar’s size mode.

Deprecated

enum SizeMode

Constants that specify toolbar display modes.

Deprecated

