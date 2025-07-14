

- AppKit
- NSToolbar
-  fullScreenAccessoryViewMaxHeight Deprecated

Instance Property

# fullScreenAccessoryViewMaxHeight

The maximum height of the toolbar’s full screen accessory view, in points.

macOS 10.7–10.13Deprecated

``` source
@MainActor
var fullScreenAccessoryViewMaxHeight: CGFloat { get set }
```

Deprecated

Use an NSTitlebarAccessoryViewController with an NSWindow instead.

## Discussion

The fullScreenAccessoryViewMaxHeight is used when displaying a fully revealed menu bar. During the reveal, the toolbar’s accessory view’s frame is interpolated between its fullScreenAccessoryViewMinHeight and `fullScreenAccessoryViewMaxHeight` properties.

By default the maximum height gets set to the height of the accessory view’s frame when it’s set.

## See Also

### Deprecated

var centeredItemIdentifier: NSToolbarItem.Identifier?

The item to display in the center of the toolbar.

Deprecated

var fullScreenAccessoryView: NSView?

The toolbar’s full screen accessory view.

Deprecated

var fullScreenAccessoryViewMinHeight: CGFloat

The minimum height of the toolbar’s full screen accessory view.

Deprecated

var sizeMode: NSToolbar.SizeMode

The toolbar’s size mode.

Deprecated

enum SizeMode

Constants that specify toolbar display modes.

Deprecated

